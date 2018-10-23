<template>
    <div>
    <section class="card" style="padding:15px;box-shadow:0 5px 15px rgba(0,0,0,.08); border-radius: 15px 15px 15px 15px;margin:auto; margin-top:2rem;">
        <center><h1 style="font-size:30px">Авторизация</h1></center>
        <br>
         <b-field>
            <b-input placeholder="Имя пользователя"
                icon="account">
            </b-input>
        </b-field>

        <b-field>
            <b-input type="password" icon="lock"
                placeholder="Пароль"
                password-reveal>
            </b-input>
        </b-field>

<div style="text-align:center;margin:0.1rem">
                <button class="button is-link" style="box-shadow: 0 8px 16px 0 rgba(0,0,0,.2), 0 6px 20px 0 rgba(0,0,0,.19);width:50%" @click="registration"><b-icon icon="account-multiple-plus"></b-icon>&nbsp;&nbsp;Войти</button>
</div>

<hr>
Еще нет аккаунта?<nuxt-link to="registration" > Зарегистрироваться</nuxt-link>
</section>
<Footer style=" position: absolute;"/>
</div>
</template>

<style scoped>
@media (min-width: 768px) { 
    .card {
        width:30%;
    }
}
</style>
<script>
import Footer from '@/components/Footer'

export default {
  name: 'HomePage',
  components: {
    Footer
  },
  data() {
      return {
      }
  }
}
</script>