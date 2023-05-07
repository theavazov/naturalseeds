<template>
  <footer class="footer">
    <div class="box inner_top">
      <span to="/" class="logo"></span>
    </div>
    <div class="bottom_wrapper">
      <div class="box inner_bottom">
        <p>При перепечатке любых материалов ссылка на веб-сайт обязательна</p>
        <p>{{ new Date().getFullYear() }}. Все права защищены.</p>
      </div>
    </div>
  </footer>
</template>

<script setup></script>

<style scoped>
.footer {
  background-color: var(--black);
  color: var(--white);
}

.inner_top {
  padding-top: 55px;
  padding-bottom: 32px;
}

.bottom_wrapper {
  border-top: 1px solid rgba(255, 255, 255, 0.4);
}

.inner_bottom {
  padding-block: 24px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 16px;
}

.inner_bottom p {
  font-size: 16px;
  line-height: 24px;
}
</style>
