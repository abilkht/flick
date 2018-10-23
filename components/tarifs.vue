<template>
  <div style="background-image: linear-gradient(135deg, #6B31C1 0%, #6E85F3 100%);">
    <h1 style="text-align:center;color:white;" class="choose-tarif">Выберите вид подписки</h1>
  <div class="row columns" style="margin:auto;padding:auto;width:80%">
    <div class="column is-one-third">
    <div class="card"  style="border-radius: 15px 15px 15px 15px;box-shadow: 0 8px 16px 0 rgba(0,0,0,.2), 0 6px 20px 0 rgba(0,0,0,.19);">
  <div class="card-image">
    <figure class="image is-4by3">
      <img src="../static/base.jpg" alt="Placeholder image" style="border-radius: 15px 15px 0px 0px;">
    </figure>
  </div>
  <div class="card-content">
    <div class="media">
      <div class="media-left">
        <figure class="image is-48x48">
          <img src="../static/battery.png" alt="Placeholder image">
        </figure>
      </div>
      <div class="media-content">
        <p class="title is-4">Базовый</p>
        <p class="subtitle is-6">2 290 тг</p>
      </div>
    </div>

    <div class="content">
      <br><b-icon icon="check-circle" style="color:#7957d5"></b-icon>Один просмотр фильма в день
      <br><b-icon icon="check-circle" style="color:#7957d5"></b-icon>5 фильмов в месяц
      <br><b-icon icon="check-circle" style="color:#7957d5"></b-icon>Билет для друга со скидкой 50%
      <br><b-icon icon="check-circle" style="color:#7957d5"></b-icon>Выбор любого места в кинотеатре
      <br>
       <br>
      <a class="button is-link level-item" style="text-align:center;" @click="registration">Выбрать</a>
    </div>
  </div>
</div>
</div>
<div class="column is-one-third">
    <div class="card" style="border-radius: 15px 15px 15px 15px;box-shadow: 0 8px 16px 0 rgba(0,0,0,.2), 0 6px 20px 0 rgba(0,0,0,.19);" >
  <div class="card-image">
    <figure class="image is-4by3">
      <img src="../static/standard.jpg" alt="Placeholder image" style="border-radius: 15px 15px 0px 0px;">
    </figure>
  </div>
  <div class="card-content">
    <div class="media">
      <div class="media-left">
        <figure class="image is-48x48">
          <img src="../static/battery(1).png" alt="Placeholder image">
        </figure>
      </div>
      <div class="media-content">
        <p class="title is-4">Стандарт</p>
        <p class="subtitle is-6">4 290 тг</p>
      </div>
    </div>

    <div class="content">
      <br><b-icon icon="check-circle" style="color:#7957d5"></b-icon>Один просмотр фильма в день
      <br><b-icon icon="check-circle" style="color:#7957d5"></b-icon>12 фильмов в месяц
      <br><b-icon icon="check-circle" style="color:#7957d5"></b-icon>Билет для друга со скидкой 50%
      <br><b-icon icon="check-circle" style="color:#7957d5"></b-icon>Выбор любого места в кинотеатре
      <br>
       <br>
      <a class="button is-link level-item" style="text-align:center;" @click="registration">Выбрать</a>
    </div>
  </div>
</div>
</div>
<div class="column is-one-third">
    <div class="card"  style="border-radius: 15px 15px 15px 15px;box-shadow: 0 8px 16px 0 rgba(0,0,0,.2), 0 6px 20px 0 rgba(0,0,0,.19);">
  <div class="card-image">
    <figure class="image is-4by3">
      <img src="../static/premium.jpg" style="border-radius: 15px 15px 0px 0px;">
    </figure>
  </div>
  <div class="card-content">
    <div class="media">
      <div class="media-left">
        <figure class="image is-48x48">
          <img src="../static/battery(2).png" alt="Placeholder image">
        </figure>
      </div>
      <div class="media-content">
        <p class="title is-4">Премиум</p>
        <p class="subtitle is-6">6 490 тг</p>
      </div>
    </div>

    <div class="content">
      <br><b-icon icon="check-circle" style="color:#7957d5"></b-icon>5 просмотров фильма в день
      <br><b-icon icon="check-circle" style="color:#7957d5"></b-icon>30 фильмов и блокбастеров в месяц
      <br><b-icon icon="check-circle" style="color:#7957d5"></b-icon>Билет для друга со скидкой 50%
      <br><b-icon icon="check-circle" style="color:#7957d5"></b-icon>Выбор лювого места в кинотеатре
      <br>
       <br>
      <a class="button is-link level-item" style="text-align:center;" @click="registration">Выбрать</a>
    </div>
  </div>
</div>
</div>
  </div>
</div>
</template>
<style scoped>
 @media (min-width: 768px) { 
    h1 {
        font-size: 3rem;
    }
}
@media (max-width: 768px) { 
    h1 {
        font-size: 2rem;
    }
}
</style>
<script>
export default {
  name: 'HomePage',
  data() {
      return {
      }
  },
  methods: {
    registration() {
      this.$router.push('registration');
    }
  }
}
</script>