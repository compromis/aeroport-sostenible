<script setup>
import BCard from '@compromis/blobby/components/card/BCard.vue'
import BInputGroup from '@compromis/blobby/components/inputs/BInputGroup.vue'
import BInput from '@compromis/blobby/components/inputs/BInput.vue'
import BCheckbox from '@compromis/blobby/components/inputs/BCheckbox.vue'
import BButton from '@compromis/blobby/components/button/BButton.vue'

function submit() {

}
</script>

<template>
  <section class="form card">
    <BCard padded shadow>
      <h2>Firma</h2>
      
      <Motion />
      
      <form @submit.prevent="submit">
        <BInputGroup class="form-group">
          <BInput variant="float" label="Nom" name="first_name" span="2" required />
          <BInput variant="float" label="Cognoms" name="last_name" span="2" required />
          <BInput variant="float" label="Email" name="email" type="email" span="4" required />
        </BInputGroup>

        <BCheckbox name="privacy" value="Accepte" required class="privacy my-4">
          Accepte la <a href="https://compromis.net/avis-legal/">política de privacitat</a> i done consentiment perquè <strong>Compromís</strong> tramite les al·legacions exposades en el meu nom.
        </BCheckbox>

        <BButton type="submit" variant="primary" size="lg">
          Firma
        </BButton>
      </form>
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

.form-group .card {
  box-shadow: none !important;
  border: 1px var(--gray-300) solid;
}

.form .button-lg {
  font-size: 1.5rem !important;
  min-height: auto !important;
}
</style>

<style lang="scss">
.hs-form__virality-link {
  display: none;
}
</style>