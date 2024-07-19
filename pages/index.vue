<script setup lang="ts">
useHead({
  htmlAttrs: {
    lang: 'ca',
  },
})

useSeoMeta({
  title: 'Aeroport sostenible - Compromís',
  ogTitle: 'Aeroport sostenible - Compromís',
  description: 'Firma per frenar l\'ampliació de vols i pistes de l\'Aeroport de Manises, per garantir la salut i el benestar de milers de persones.',
  ogDescription: 'Firma per frenar l\'ampliació de vols i pistes de l\'Aeroport de Manises, per garantir la salut i el benestar de milers de persones.',
  ogImage: 'https://aeroportsostenible.compromis.net/images/ogimage.png',
  twitterCard: 'summary_large_image',
})

const accordion = [
  {
    number: 'material-symbols:person-pin',
    title: 'Els protagonistes',
    text: [
      'Aena, empresa pública participada en un 49% per socis privats des de 2015, vol augmentar el nombre de vols a l’Aeroport de València per incrementar els seus ingressos per taxes. Aquesta proposta compta amb el suport del President Carlos Mazón <sup class="pp">(PP)</sup> i de la Consellera Nuria Montes <sup class="pp">(PP)</sup>, així com del Ministre de Tranports, Óscar Puente <sup class="psoe">(PSOE)</sup>, el mateix que dona suport a l’ampliació del Port sense realitzar una nova Declaració d’Impacte Ambiental.',
      'Des de la Diputació d\'Alacant i el seu Patronat de Turisme, Mazón, i des de la gerència de la patronal de turisme HOSBEC, Montes, abans de les eleccions de 2023 varen concertar amb els tour operadors més forts anglesos i americans, la vinguda massiva de turistes de sol i platja, majoritàriament de low-cost, a través de paquets tancats de vol i hotel. Ara demanen una ampliació impossible per aconseguir més vols, més passatgers i més clients per als negocis dels seus amics i socis.'
    ]
  },
  {
    number: 'mdi:bar-chart',
    title: 'Les xifres',
    text: [
      'L’Aeroport de Manises, en l’actualitat, té un volum mensual de 7.852 operacions d’aeronaus (maig 2024): 5.090 durant el dia, 1.659 per la vesprada i 1.103 per la nit, entre les 23:00 h. i les 7:00 h. L’Aeroport opera les 24 hores del dia.',
      'Això suposa una greu contaminació acústica que es pot doblar si a partir de 2027 es posa en marxa una nova pista i augmenta el nombre de vols per satisfer els interessos dels operadors. AENA ha hagut de pagar la insonorització de milers de vivendes perquè els nivells de soroll superen els mínims legals. És una situació insostenible. Afecta a una població superior a les 500.000 persones que viuen a Manises, Quart de Poblet, Aldaia, Barri del Crist, Mislata, Xirivella, Riba roja de Túria i València (essencialment Patraix).'
    ]
  },
  {
    number: 'octicon:mute-24',
    title: 'Pla d\'acció contra el soroll',
    text: [
      'La Dirección General de Aviación Civil ha publicat un Pla contra el Soroll de l’Aeroport de València que es troba ara en fase d’al·legacions. Servirà com a justificació per promoure una ampliació de vols i pistes que hem de frenar.',
      'Per això, et demanem el teu suport firmant el text que pots llegir a continuació. El Pla presenta diverses deficiències importants que han de ser abordades per complir amb la normativa europea i garantir la protecció dels residents de les poblacions afectades.',
    ]
  },
]
</script>

<template>
  <main>
    <div class="container">
      <SiteHeader>
        <SiteTitle />
      </SiteHeader>
      <section class="text text-intro">
        <h1 v-motion-fade-visible class="visually-hidden">
          Aeroport sostenible
        </h1>

        <Languages />

        <p v-motion-fade-visible>
          Firma per frenar l'ampliació de vols i pistes de l'Aeroport de Manises, per garantir la salut i el benestar de milers de persones
        </p>
 
        <p v-motion-fade-visible>
          1.103 operacions nocturnes d'aeronaus <sup>(maig de 2024)</sup>, un turisme de baixa qualitat que trenca el mercat de la vivenda ocupant apartaments majoritàriament il·legals, una població afectada que ha de tancar les seues finestres per poder descansar
        </p>
      </section>
    </div>
    <Accordion id="accordtion" :content="accordion" />
    <SiteForm />
    <Share>
      <template #title>Fes-ne difusió!</template>
      <p>Comparteix aquesta pàgina amb les teues amistats.</p>
    </Share>
  </main>
</template>
