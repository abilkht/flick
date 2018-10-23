<template>
  <div>
    <nav class="navbar is-transparent" style="box-shadow: 0 0 10px rgba(0,0,0,0.5);background-image: linear-gradient(135deg, #6B31C1 0%, #6E85F3 100%);">
  <div class="navbar-brand">
    <nuxt-link class="navbar-item" to="/">
      <img src="../static/logo.png" >&nbsp;<p style="font-size:1rem;font:bold;color:white;font-family:Montserrat,Helvetica Neue,Helvetica,Arial,sans-serif">flick</p>
    </nuxt-link>

        <div class="navbar-burger" @click="showNav = !showNav" :class="{ 'is-active': showNav }" style="color:white;">
          <span></span>
          <span></span>
          <span></span>
        </div>
  </div>

  <div class="navbar-menu" :class="{ 'is-active': showNav }" style="background-image: linear-gradient(135deg, #6B31C1 0%, #6E85F3 100%);">
    <div class="navbar-end">
      <div class="navbar-item">
        <div class="field is-grouped">
          
          <nuxt-link to="/registration" class="navbar-item" style=" color:white;">
            <p id="nav-menu"> Начать</p>
          </nuxt-link>

          <nuxt-link to="/login" class="navbar-item" id="icon-nav" style=" color:white;">
            <p id="nav-menu"><b-icon icon="account"></b-icon>&nbsp;Вход</p>
          </nuxt-link>

        </div>
      </div>
    </div>
  </div>
</nav>
      <div>
        <nuxt/>
      </div>


        
  </div>
</template>
<style>

h1,p,h2,h3 {
  font-family: Montserrat,Helvetica Neue,Helvetica,Arial,sans-serif;
}
  .facebook:hover, .vk:hover {
    background-color: #4267b2
  }
  .instagram:hover {
    background-color: #ea4c89
  }
  nuxt-link {
    color:white;
  }
/*  @media (min-width: 768px) { */
/*    #nav-menu{
      color:white;
    }
    #icon-nav {
      color:white;
    }
}
  @media (max-width: 768px) { 
    #nav-menu, span {
      color:black;
    }

}*/

</style>
<script>
export default {
  data() {
    return {
      showNav: false,
      items: [
        { title: 'Home', icon: 'home', to: { name: 'index' } },
        { title: 'Inspire', icon: 'lightbulb', to: { name: 'inspire' } }
      ]
    }
  }
}
</script>