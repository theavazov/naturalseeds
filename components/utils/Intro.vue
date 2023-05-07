<template>
  <section class="section">
    <nav class="box section_nav">
      <nav class="breadcrumb">
        <nuxt-link to="/" class="breadcrumb_element">Главная</nuxt-link>
        <span class="breadcrumb_element">/</span>
        <p class="breadcrumb_element">{{ title }}</p>
      </nav>
      <h1 class="page_title">{{ title }}</h1>
    </nav>
  </section>
</template>

<script lang="ts">
export default defineComponent({
  props: ["title"],
});
</script>

<style scoped>
.section {
  background: var(--bg-gradient);
}

.section_nav {
  display: flex;
  flex-direction: column;
  gap: 16px;
  padding-top: 72px;
  padding-bottom: 64px;
}

.breadcrumb {
  display: flex;
  align-items: center;
  gap: 8px;
}

.breadcrumb_element {
  font-size: 16px;
  line-height: 20px;
  color: var(--white);
}

a.breadcrumb_element {
  font-size: 16px;
  line-height: 20px;
  opacity: 0.56;
  transition: 0.3s;
}

a.breadcrumb_element:hover {
  opacity: 1;
  transition: 0.3s;
}
</style>
