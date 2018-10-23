<template>
  <div style="border-bottom:1px solid #e9e1df;">
  <div class="container">
     <h1 style="text-align:center;margin-bottom:1rem;" class="choose-tarif">Как это работает?</h1>
  <div class="columns">
  <div class="column credit-card-column">
    <img src="../static/credit-card.png" class="credit-card">
  </div>

  <div class="column">
   
   <div class="card" style="border-radius: 15px 15px 15px 15px;box-shadow: 0 8px 16px 0 rgba(0,0,0,.2), 0 6px 20px 0 rgba(0,0,0,.19);margin-bottom:1rem">
  <div class="card-content">
    <div class="media">
      <div class="media-left">
        <figure class="image is-48x48">
          <img src="../static/first-step.png" alt="Placeholder image">
        </figure>
      </div>
      <div class="media-content">
        <p class="title is-4">№1. Регистрация</p>
        <p class="subtitle is-6" style="font-size:14px;">&nbsp;3-5 минут</p>
      </div>
    </div>

    <div class="content">
      Вы создаете новую учетную запись и заполняете свои данные. 
      <br>
      <a>Зарегистрироваться</a>
      <br>
    </div>
  </div>
</div>
<div class="card" style="border-radius: 15px 15px 15px 15px;box-shadow: 0 8px 16px 0 rgba(0,0,0,.2), 0 6px 20px 0 rgba(0,0,0,.19);margin-bottom:1rem">
  <div class="card-content">
    <div class="media">
      <div class="media-left">
        <figure class="image is-48x48">
          <img src="../static/second-step.png" alt="Placeholder image">
        </figure>
      </div>
      <div class="media-content">
        <p class="title is-4">№2. Получение подписки</p>
        <p class="subtitle is-6" style="font-size:14px">1-3 минуты</p>
      </div>
    </div>

    <div class="content">
      Оформляете подходящую вам подписку.
      <br>
      <br>
    </div>
  </div>
</div>
<div class="card" style="border-radius: 15px 15px 15px 15px;box-shadow: 0 8px 16px 0 rgba(0,0,0,.2), 0 6px 20px 0 rgba(0,0,0,.19);margin-bottom:1rem">
  <div class="card-content">
    <div class="media">
      <div class="media-left">
        <figure class="image is-48x48">
          <img src="../static/third-step.png" alt="Placeholder image">
        </figure>
      </div>
      <div class="media-content">
        <p class="title is-4">№3. Выбор кинофильма</p>
        <p class="subtitle is-6" style="font-size:14px">от 1 часа</p>
      </div>
    </div>

    <div class="content">
      Выбираете себе подходящий кинотеатр и фильм. 
      <br>
      <br>
    </div>
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
        font-size: 1.5rem;
    }
    .card {
      width:90%;
      margin:auto;
    }
    .credit-card {
      width: 70%;
      height: 70%;
    }
    .credit-card-column {
      margin-left:4rem;
    }
}
</style>