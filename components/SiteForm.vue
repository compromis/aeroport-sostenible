<script setup>
onMounted(() => {
  window.hbspt.forms.create({
    region: "eu1",
    portalId: "145034122",
    formId: "c3421965-2509-4637-a6aa-19f46dc9a6de",
    target: "#hubspotForm"
  })
})
</script>

<template>
  <section class="form">
    <div id="hubspotForm" />
  </section>
</template>

<style lang="scss" scoped>
.form {
  padding: var(--site-padding);
  border-radius: 1rem;
  overflow: hidden;
  max-width: 1300px; 
  margin: 0 auto;
}
</style>