<template>
  <LazyUtilsForm />
  <section class="partners_section">
    <div class="box section_inner">
      <h3 class="section_title">Наши партнёры</h3>
    </div>
  </section>
</template>

<script lang="ts" setup>
useHead({ title: "«Natural SEEDS»- крупная семеноводческая компания." });
</script>

<style scoped>
.section_inner {
  display: flex;
  flex-direction: column;
  gap: 32px;
}

.partners_section {
  position: relative;
  padding-block: 120px;
}
</style>
