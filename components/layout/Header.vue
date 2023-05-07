<template>
  <header class="header">
    <div class="box header_inner">
      <div class="inner_top">
        <div class="main_nav">
          <nuxt-link to="/" class="logo" title="home"></nuxt-link>
          <p>большой выбор эксклюзивных семен</p>
        </div>
        <div class="extra_nav"></div>
      </div>
    </div>
    <div class="navigation_wrapper">
      <nav class="box navigation">
        <nuxt-link to="/" class="nav_link">Главная</nuxt-link>
        <button class="nav_link">Продукции</button>
        <nuxt-link to="/about" class="nav_link">О компании</nuxt-link>
        <nuxt-link to="/technologies" class="nav_link"
          >Технологии и оборудования</nuxt-link
        >
        <nuxt-link to="/news" class="nav_link">Новости</nuxt-link>
        <nuxt-link to="/contacts" class="nav_link">Контакты</nuxt-link>
        <button class="nav_link">Русский</button>
      </nav>
    </div>
  </header>
</template>

<script setup></script>

<style scoped>
.header {
  position: fixed;
  top: 0;
  width: 100%;
  z-index: 4;
  background-color: var(--white);
}

.header_inner {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 24px;
  padding-block: 20px;
}

.main_nav {
  display: flex;
  align-items: center;
  gap: 30px;
}

.main_nav p {
  font-size: 16px;
  line-height: 24px;
  color: rgba(75, 76, 88, 0.56);
  max-width: 212px;
}

.navigation_wrapper {
  border-block: 1px solid rgba(2, 1, 5, 0.16);
}

.navigation {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 24px;
  padding-block: 20px;
}

.nav_link {
  font-size: 16px;
  line-height: 20px;
  color: var(--black);
  display: flex;
  align-items: center;
  gap: 6px;
  transition: 0.3s;
}

.nav_link svg {
  max-width: 18px;
  widows: 100%;
  height: 18px;
}

.nav_link:hover {
  color: var(--green);
  transition: 0.3s;
}

.router-link-exact-active {
  color: var(--green);
  font-weight: 600;
  transition: 0.3s;
}
</style>
