<template>
	<div style="border-bottom:1px solid #e9e1df;">
	 <div class="container" >
	   <div class="columns">
        <div class="column is-one-third" id="descrip" style="margin:auto;">
          <div style="margin:auto;">
            <h1><b>Широкий выбор кинотеатров</b></h1>
            <small>Мы сотрудничаем c <b>8 кинотеатрами Астаны</b>. Вы сможете посещать ближайщий вам кинотеатр</small>
          </div>
        </div>
        <div class="column">
           <img src="../static/cinema.png">
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped>
img {
   -moz-transform: scaleX(-1);
        -o-transform: scaleX(-1);
        -webkit-transform: scaleX(-1);
        transform: scaleX(-1);
        filter: FlipH;
        -ms-filter: "FlipH";
}

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