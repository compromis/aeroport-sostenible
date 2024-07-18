<script setup>
import BCard from '@compromis/blobby/components/card/BCard.vue'
import BInputGroup from '@compromis/blobby/components/inputs/BInputGroup.vue'
import BInput from '@compromis/blobby/components/inputs/BInput.vue'
import BCheckbox from '@compromis/blobby/components/inputs/BCheckbox.vue'
import BButton from '@compromis/blobby/components/button/BButton.vue'

const props = defineProps({
  cas: { type: Boolean, default: false }
})

const errors = ref(null)
const submitted = ref(false)
const submitting = ref(false)
const form = reactive({
  first_name: '',
  last_name: '',
  email: '',
  privacy: false
})

async function submit() {
  try {
    await $fetch('https://forms.compromis.net/api/forms/aeroport-sostenible', {
      method: 'POST',
      body: form
    })
    submitted.value = true
  } catch(e) {
    errors.value = e
  } finally {
    submitting.value = false
  }
}

const strings = {
  val: {
    title: 'Firma contra l\'ampliació de l\'Aeroport de Manises',
    first_name: 'Nom',
    last_name: 'Cognoms',
    button: 'Firma'
  },
  cas: {
    title: 'Firma contra la ampliación del Aeropuerto de Manises',
    first_name: 'Nombre',
    last_name: 'Apellidos',
    button: 'Firmar'
  }
}

const t = computed(() => props.cas ? strings.cas : strings.val)
</script>

<template>
  <section class="form card">
    <BCard padded shadow>
      <h2>{{ t.title }}</h2>
      
      <Motion :cas="cas" />
      
      <form v-if="!submitted" @submit.prevent="submit">
        <BInputGroup class="form-group">
          <BInput v-model="form.first_name" variant="float" :label="t.first_name" name="first_name" span="2" required />
          <BInput v-model="form.last_name" variant="float" :label="t.last_name" name="last_name" span="2" required />
          <BInput v-model="form.email" variant="float" label="Email" name="email" type="email" span="4" required />
        </BInputGroup>

        <BCheckbox v-model="form.privacy" name="privacy" value="Accepte" required class="privacy my-4">
          <template v-if="cas">
            Acepto la <a href="https://compromis.net/avis-legal/">política de privacidad</a> y doy consentimiento para que <strong>Compromís</strong> tramite las alegaciones expuestas en mi nombre.
          </template>
          <template v-else>
            Accepte la <a href="https://compromis.net/avis-legal/">política de privacitat</a> i done consentiment perquè <strong>Compromís</strong> tramite les al·legacions exposades en el meu nom.
          </template>
        </BCheckbox>

        <BButton type="submit" variant="primary" size="lg" :disabled="submitting">
          {{ t.button }}
        </BButton>
      </form>
      <div v-else class="submitted gradient-secondary bg-gradient rounded-md">
        <template v-if="cas">
          <h2 class="mb-4">Firma recibida</h2>
          <p>Gracias por firma por un aeropurto más sostenible.</p>
          <p class="mb-0"><a href="#share">Comparte esta página</a> con tus amistades para que llegue a más gente</p>
        </template>
        <template v-else>
          <h2 class="mb-4">Signatura rebuda!</h2>
          <p>Gràcies per signar per un aeroport més sostenible!</p>
          <p class="mb-0"><a href="#share">Comparteix aquesta pàgina</a> amb les teues amistats per arribar a més gent!</p>
        </template>
      </div>
    </BCard>
  </section>
</template>

<style lang="scss">
.form {
  padding: var(--site-padding);
  border-radius: 1rem;
  overflow: hidden;
  max-width: var(--text-container);
  margin: 0 auto;
}

.input-float .input {
  border-radius: 0;
}

.form-group .card {
  box-shadow: none !important;
  border: 1px var(--gray-300) solid;
}

.form .button-lg {
  font-size: 1.5rem !important;
  min-height: auto !important;
}

.submitted {
  color: var(--white);
  padding: 1rem;

  a {
    color: var(--white);
    text-decoration: underline;
  }
}
</style>

<style lang="scss">
.hs-form__virality-link {
  display: none;
}
</style>