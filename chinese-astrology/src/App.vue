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
            <div v-for="service of services" :key="service.name" class="service__item-wrapper">
              <img class="service__item-image" src="../img/photo_2023-12-19_17-12-07.jpg" alt="">
              <h3 class="service__item-h3">{{ service.name }}</h3>
              <p class="service__item-description">
                {{ service.description }}
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </main >
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      services: [
        {
          name: "Любовь в 2024 году",
          description: "У каждого из нас бывают периоды, когда в нашей карте Бацзы затрагивается Дом Брака" + "Дом Брака — второй столп в карте под названием «День» или «Личность»"
        },
        {
          name: "Развод в 2024",
          description: "Зона риска в 2024г в отношениях"
        },
        {
          name: "Здоровье в 2024",
          description: "Многих волнуют вопросы:"+
                      "– какие болезни могут активизироваться?" +
                      "– каким органам стоит уделить внимание" +
                      "– кто будет в зоне риска и кому стоит выделить тему здоровья в своём планере на год"
        },
        {
          name: "Прогноз по элементам",
          description: "Ежедневно выкладывается прогноз на день для всех элементов, но Вы также  можете более подробно узнать для себя"
        },
        {
          name: "События в 2024",
          description: "Что ждет нас в грядущем году"
        },
        {
          name: "Грабитель богатства",
          description: "Дни грабителя — это дни, когда деньги могут уйти из вашего кошелька. Поэтому рекомендуется самим запланировать траты, чтобы финансы не ушли сами собой."
        }
      ]
    }
  }
}
</script>

<style lang="scss" src="./style/App.scss">
</style>
