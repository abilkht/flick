<template class="is-widescreen">
  <div >
<div>
    <section class="section is-widescreen" >
      <div class="container" style="">
        <p style="font-weight: 600; line-height: 1.2; text-align: center;color:white;width:60%;margin-right:auto;margin-left:auto;" class="header">Упрощаем покупку билетов в кинотеатры до месячной подписки</p>
       <div class="level-item" style="margin:1rem">
        <a class="button is-primary subtitle" style="overflow: auto;background-image: linear-gradient(135deg, #6B31C1 0%, #6E85F3 100%);margin-top:1rem;margin-bottom:1.5rem;box-shadow:0 8px 16px 0 rgba(0,0,0,.2), 0 6px 20px 0 rgba(0,0,0,.19);" id="button-start" @click="registration">Начать</a>
      </div>

    </div>
    </section>
    <Description/>
    
    </div>
    <Cons/>
    <Partners/>
    <Anytime/>
    <tarifs/>
    <Faq/>
    <Footer/>
</div>
</template>


<style scoped>
section {
  background-image: url('../static/novocinema1.jpg');
  background-repeat: no-repeat;
  background-position: center; 
   -webkit-background-size: cover;
        -moz-background-size: cover;
        -o-background-size: cover;
background-size: cover;

}
@media (min-width: 768px) { 
    p {
        font-size: 3em;
        width:60%;
    }
    .container {
      margin-top:8em;
      margin-bottom:8em;
    }
        #button-start{
            width:20%;
        }
}
@media (max-width: 768px) { 
    p {
        font-size: 2em;
    }
    .container {
      margin-top:2em;
      margin-bottom:2em;
    }
        .start {
            width:90%;
            margin:auto;
        }    
}
</style>
<script>
import tarifs from '@/components/tarifs'
import Faq from '@/components/Faq'
import Partners from '@/components/Partners'
import Anytime from '@/components/Anytime'
import Description from '@/components/Description'
import Footer from '@/components/Footer'
import Cons from '@/components/Cons'
import Steps from '@/components/Steps'
export default {
  name: 'HomePage',
  components: {
    tarifs,
    Footer,
    Cons,
    Steps,
    Description,
    Faq,
    Partners,
    Anytime
  },
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

