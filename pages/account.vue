<template>
<div>
<section  v-if="isFullPage">

  <h1 style="text-align:center;font-size:2rem;">Мой аккаунт</h1>
  <div style="width:50%;margin-left:auto;margin-right:auto;margin-top:2rem;">
    <div class="columns">
        <div class="column card" style="padding:15px; border-radius: 15px 15px 15px 15px;margin-right:1rem;" id="column-card">
        <h6><b>Сделайте свой первый заказ <a>прямо сейчас</a></b></h6>
        <small> <font style="opacity:0.7">Вы не производили оплату в этом месяце.</font> <br>
        <b>Стартовый</b> - 5000 тг.<br>
        <b>Стандартный</b> - 9 000 тг.<br>
        <b>Премиум</b> - 18 000 тг.</small>
        <button class="button is-link" style="box-shadow: 0 8px 16px 0 rgba(0,0,0,.2), 0 6px 20px 0 rgba(0,0,0,.19);margin-top:1.5rem;width:100%;padding:3px"><b-icon icon="ticket-account"></b-icon>&nbsp;&nbsp;Приобрести подписку</button>
        <p style="text-align:center;margin-top:1.5rem;">ZqxuNs31EcT2</p>
        <small>Поделитесь этим кодом с другом. Он получит скидку в 500тг.
        Как только он подпишется, скидка будет у вас.</small>
        <br>
        <a style="margin-top:2rem;font-size:0.8rem">У вас есть промокод?</a>
        <button class="button is-link" style="box-shadow: 0 8px 16px 0 rgba(0,0,0,.2), 0 6px 20px 0 rgba(0,0,0,.19);margin-top:1.5rem;width:100%;padding:3px"><b-icon icon="gift"></b-icon>&nbsp;&nbsp;Потратить бонусы</button>
    </div>

     <div div class="column card" style="padding:15px; border-radius: 15px 15px 15px 15px;margin-left:1rem;">
        <strong><b-icon icon="account"></b-icon>&nbsp;&nbsp;Темирлан Нурланов</strong><br>
        <small><b-icon icon="email"></b-icon>&nbsp;&nbsp;tema.nurlanov@gmail.com</small><br>

<small><b-icon icon="cellphone"></b-icon>&nbsp;&nbsp;+7 (700) 423 88 12</small><br>

<small><b-icon icon="city"></b-icon>&nbsp;&nbsp;Есенина 2, Астана</small><br>

<small><b-icon icon="call-merge"></b-icon>&nbsp;&nbsp;Стартовый</small><br>

<button class="button" style="text-align:center;margin-top:1rem;width:100%" @click="open">Изменить информацию</button><br>
 <br> <br> <br> <br>
Поделитесь о нас<br>
<a> <b-icon icon="vk"></b-icon>VKontakte</a><br>
 <a><b-icon icon="facebook"></b-icon>Facebook</a><br>
 <a><b-icon icon="whatsapp"></b-icon>Whatsapp</a><br>
    </div>
  </div>
</div>
    </section>
<Footer style=" position: absolute;"/>
</div>
</template>
<style scoped>
.card:hover {
  box-shadow:0 5px 15px rgba(0,0,0,.9); border-radius: 45px 45px 45px 45px;
}
</style>
<script>
import Footer from '@/components/Footer'
export default {
        data() {
            return {
                isFullPage: true,
                showContent:false
            }
        },
         components: {
          Footer
        },
        created() {
            let vm = this
            const loadingComponent = this.$loading.open({

                    container: this.isFullPage ? null : this.$refs.element.$el
                    
                })
                setTimeout(() => loadingComponent.close(), 1 * 1000)
}
    }
</script>