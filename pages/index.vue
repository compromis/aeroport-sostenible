<script setup lang="ts">
useHead({
  htmlAttrs: {
    lang: 'ca',
  },
})

useSeoMeta({
  title: 'El mapa de la vergonya - Compromís',
  ogTitle: 'El mapa de la vergonya - Compromís',
  description: 'Una ferramenta viva on podreu identificar com ens afecten de manera concreta eixes polítiques al llarg del País Valencià: punts negres, retallades, caos, inoperància i censura.',
  ogDescription: 'Una ferramenta viva on podreu identificar com ens afecten de manera concreta eixes polítiques al llarg del País Valencià: punts negres, retallades, caos, inoperància i censura.',
  ogImage: 'https://mapavergonya.compromis.net/images/ogimage.png',
  twitterCard: 'summary_large_image',
})
</script>

<template>
  <main>
    <div class="container">
      <SiteHeader />
      <section class="text text-intro">
        <h1 v-motion-fade-visible class="visually-hidden">
          Aeroport sostenible
        </h1>

        <Languages />

        <p v-motion-fade-visible>
          Firma per frenar l'ampliació de vols i pistes de l'Aeroport de Manises, per garantir la salut i el benestar de milers de persones
        </p>
 
        <p v-motion-fade-visible>
          1.103 operacions d'aeronaus nocturnes (maig de 2024), un turisme de baixa qualitat que trenca el mercat de la vivenda ocupant apartaments majoritàriament il·legals, una població afectada que ha de tancar les seues finestres per poder descansar
        </p>
      </section>
    </div>
    <SiteForm />
    <Share>
      <template #title>Fes difusió!</template>
      <p>Comparteix aquesta pàgina amb les teues amistats.</p>
    </Share>
  </main>
</template>
