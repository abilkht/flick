<template>
    <div>
        <section class="section" >
            <h1 style="text-align:center;">Так в чем подвох?</h1>
<center><small style="text-align:center;">Его нет. Серьезно. Никаких дополнительных контрактов, мелкого шрифта и прочей чепухи. Остались вопросы? Читайте:</small></center><br>


         <b-collapse class="card" :open="false" style="border-radius: 15px 15px 15px 15px;margin-bottom:1rem">
            <div slot="trigger" slot-scope="props" class="card-header" style="border-radius: 15px 15px 15px 15px;">
                <p class="card-header-title" style="border-radius: 15px 15px 15px 15px;">
                    За что еще мне нужно платить кроме подписки?
                </p>
                <a class="card-header-icon" style="border-radius: 15px 15px 15px 15px;">
                    <b-icon
                        :icon="props.open ? 'menu-down' : 'menu-up'">
                    </b-icon>
                </a>
            </div>
            <div class="card-content">
                <div class="content">
                    Только за подписку. Стоимость не зависит от того, сколько вы заказали.
                    
                </div>
            </div>
        </b-collapse>
                <b-collapse class="card" :open="false" style="border-radius: 15px 15px 15px 15px;margin-bottom:1rem">
            <div slot="trigger" slot-scope="props" class="card-header" style="border-radius: 15px 15px 15px 15px;">
                <p class="card-header-title" style="border-radius: 15px 15px 15px 15px;">
                    Какие кинотеатры поддерживает Flick?
                </p>
                <a class="card-header-icon" style="border-radius: 15px 15px 15px 15px;">
                    <b-icon
                        :icon="props.open ? 'menu-down' : 'menu-up'">
                    </b-icon>
                </a>
            </div>
            <div class="card-content">
                <div class="content">
                    Приложение Flick и веб-сайт имеют карту, которая показывает ближайшие участвующие театры в вашем почтовом индексе.
                </div>
            </div>
        </b-collapse>
        <b-collapse class="card" :open="false" style="border-radius: 15px 15px 15px 15px;margin-bottom:1rem">
            <div slot="trigger" slot-scope="props" class="card-header" style="border-radius: 15px 15px 15px 15px;">
                <p class="card-header-title" style="border-radius: 15px 15px 15px 15px;">
                    Можно ли использовать Flick для просмотра любого фильма?
                </p>
                <a class="card-header-icon" style="border-radius: 15px 15px 15px 15px;">
                    <b-icon
                        :icon="props.open ? 'menu-down' : 'menu-up'">
                    </b-icon>
                </a>
            </div>
            <div class="card-content">
                <div class="content">
                    Да, при условии, что это стандартный 2D-показ - Flick позволит вам увидеть любой фильм, который не является 3D или IMAX.
                </div>
            </div>
        </b-collapse>
        <b-collapse class="card" :open="false" style="border-radius: 15px 15px 15px 15px;margin-bottom:1rem">
            <div slot="trigger" slot-scope="props" class="card-header" style="border-radius: 15px 15px 15px 15px;">
                <p class="card-header-title" style="border-radius: 15px 15px 15px 15px;">
                    Работает ли он в театрах с зарезервированными местами для сидения?
                </p>
                <a class="card-header-icon" style="border-radius: 15px 15px 15px 15px;">
                    <b-icon
                        :icon="props.open ? 'menu-down' : 'menu-up'">
                    </b-icon>
                </a>
            </div>
            <div class="card-content">
                <div class="content">
                   Да. Ваша карта MoviePass действует как обычная дебетовая карта. Не имеет значения, зарезервированы ли места для отдыха.
                   
                </div>
            </div>
        </b-collapse>
        <b-collapse class="card" :open="false" style="border-radius: 15px 15px 15px 15px;margin-bottom:1rem">
            <div slot="trigger" slot-scope="props" class="card-header" style="border-radius: 15px 15px 15px 15px;">
                <p class="card-header-title" style="border-radius: 15px 15px 15px 15px;">
                    Как далеко вперед я должен зарезервировать билет? Могу я просто использовать его по прихоти?
                </p>
                <a class="card-header-icon" style="border-radius: 15px 15px 15px 15px;">
                    <b-icon
                        :icon="props.open ? 'menu-down' : 'menu-up'">
                    </b-icon>
                </a>
            </div>
            <div class="card-content">
                <div class="content">
                    Нет конкретных временных рамок, когда вы должны использовать MoviePass. Просто используйте его так же, как и любая другая дебетовая карта.
                </div>
            </div>
        </b-collapse>
        </section>
        <div style="text-align:center;" class="start">
            <p>Мы ответили на все ваши вопросы? Тогда начинаем.</p>
            <a class="button is-primary subtitle" style="overflow: auto;background-image: linear-gradient(135deg, #6B31C1 0%, #6E85F3 100%);margin-top:1rem;margin-bottom:1.5rem;box-shadow:0 8px 16px 0 rgba(0,0,0,.2), 0 6px 20px 0 rgba(0,0,0,.19);" id="button-start" @click="registration">Начать</a>
        </div>
    </div>
</template>
<style scoped>
    @media (min-width: 768px) { 
        section {
            width:80%;
            margin:auto;
        }
        h1 {
            font-size: 1.8rem;
        }
        #button-start{
            width:20%;
        }

    }
    @media (max-width: 768px) { 
        section {
            width:95%;
            margin:auto;
        }
        .start {
            width:90%;
            margin:auto;
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