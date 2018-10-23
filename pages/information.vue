<template>
    <div>
    <section  class="card" style="padding:15px;box-shadow:0 5px 15px rgba(0,0,0,.08); border-radius: 15px 15px 15px 15px;margin:auto; margin-top:2rem;">
        <h3 class="subtitle" style="text-align: center;font-size: 30px">Информация:</h3>
        <b-field>
            <b-input placeholder="Имя"
                type="name"
                icon="account">
            </b-input>
        </b-field>

         <b-field>
            <b-input placeholder="Мобильный номер"
                type="tel"
                icon="cellphone">
            </b-input>
        </b-field>

        <b-field>
            <b-input placeholder="Адресная строка"
                icon="home">
            </b-input>
        </b-field>
        <b-field>
            <b-input placeholder="Почтовый индекс"
                icon="mailbox">
            </b-input>
        </b-field>

         <b-field>
            <b-input placeholder="Город"
                icon="city">
            </b-input>
        </b-field>
       

 <div style="text-align:center;margin:0.1rem">
                <button class="button is-link" style="box-shadow: 0 8px 16px 0 rgba(0,0,0,.2), 0 6px 20px 0 rgba(0,0,0,.19);width:50%" @click="saveInformation"><b-icon icon="check"></b-icon>&nbsp;&nbsp;Сохранить</button>
            </div>




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
        isFullPage: true
      }
  },
  created() {
            const loadingComponent = this.$loading.open({
                    container: this.isFullPage ? null : this.$refs.element.$el
                })
                setTimeout(() => loadingComponent.close(), 0.5 * 1000)
},
    methods: {
    saveInformation() {
      this.$router.push('account');
    }
  }
}
</script>