<template>
  <header>
    <div class="header__bg">
      <div class="container">
        <div class="header__wrapper">
          <div class="header__menu">
            <ul>
              <li class="header__menu-item"><a class="header__menu-link" href="">Главная</a></li>
              <li class="header__menu-item"><a class="header__menu-link" href="">О бацзы</a></li>
            </ul>
          </div>
          <div class="header__content">
            <h2 class="header__h2">Познай себя сквозь призму китайской метафизики</h2>
          </div>
        </div>
      </div>
    </div>
  </header>


  <main >
    <div class="services__wrapper">
      <div class="container">
        <div class="services__content">
          <h2 class="services__h2">Услуги</h2>
          <div class="services">
            <ServiceList />
          </div>
        </div>
      </div>
    </div>
  </main >
</template>

<script setup>
  import ServiceList from './components/ServiceList.vue';
</script>

<style lang="scss" src="./style/App.scss">
</style>
