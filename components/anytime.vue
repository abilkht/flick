<template>
	<div style="border-top:1px solid #e9e1df;">
	 <div class="container" style="">
	   <div class="columns">
       <div class="column" >
<!--            <img src="../static/time.png"  style=""> -->
          <img src="../static/calendar.png" >
        </div>
        <div class="column" id="descrip" style="margin:auto;">
          <div class="description">
            <h1><b>Круглосуточный просмотр фильмов</b></h1>
            <small style="width:70%;">Пользуясь привилегиями подписки, вы получите возможность <b>бесплатно посещать фильмы</b> в любой день недели.</small>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped>
@media (min-width: 768px) { 
    h1 {
        font-size: 2rem;
        text-align: center;
    }
     small {
      text-align: center;
      font-size:;
    }
    .description {
      margin:auto;
    }
}
@media (max-width: 768px) { 
    h1 {
        font-size: 1rem;
        width:90%;
        text-align: center;
    }
    small {
      text-align: center;
    }
    #descrip {
      width:80%;
      margin-top:1rem;
    }
    .description {
       margin-bottom:1rem;
    }
}
</style>