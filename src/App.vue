<template>
  <div id="app">
    <div class="header">
      <div class="top">

        <Logo />

        <h1><span class="red">Crypto</span>Factory<b>bot</b></h1>
        <p class="caption">Make your own crypto world in few touch</p>
        <div id="nav">
          <router-link 
            to="/promo" 
            class="link">Promo</router-link>
          <router-link 
            to="/services" 
            class="link">Services</router-link>
          <router-link 
            to="/documentation" 
            class="link">Documentation</router-link>
        </div>
        <div id="socials">
          <i class="fa fa-twitter" aria-hidden="true"></i>
          <i class="fa fa-facebook-official" aria-hidden="true"></i>
          <i class="fa fa-instagram" aria-hidden="true"></i>
        </div>
      </div>
      <router-view />
    </div>
  </div>
</template>

<script>
import Logo from './components/Logo.vue'

export default {
  name: 'App',
  components: {
    Logo
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Poppins', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: right;
  margin-top: 60px;
}
.top {
  width: 100%;
  height: 251px;
  padding-right: 120px;
  
  h1 {
    font-style: normal;
    font-weight: 400;
    font-size: 38px;
    line-height: 38px;
    text-align: right;
    letter-spacing: 0.05em;
    text-transform: uppercase;
    margin: 22px 0 0;

    .red {
      color: #E79D76;
    }
  }
  .caption {
    font-weight: 300;
    font-size: 19.5px;
    line-height: 29px;
    text-align: right;
    letter-spacing: 0.033em;
    margin: 0;
  }
  #nav {
    width: 50%;
    display: inline-block;    
    text-align: right;
    padding-right: 62px;

    a {
      display: inline-block;
      margin-left: 42px;
    }
  }
  #socials {
    display: inline-block;
    width: 172px;
    font-size: 22px;
    color: #E79D76;
    letter-spacing: 35px;
  }
}
</style>
