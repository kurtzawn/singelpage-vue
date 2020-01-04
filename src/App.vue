<template>
  <div id="app">
    <div class="container">
        <nav class="navbar nav" role="navigation" aria-label="main navigation">
        <div class="navbar-brand">
          <a class="navbar-item" href="https://bulma.io">
            <img src="https://bulma.io/images/bulma-logo.png" width="112" height="28">
          </a>

          <a role="button" class="navbar-burger burger" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
          </a>
        </div>

        <div  id="navbarBasicExample" class="navbar-menu">
          <div class="navbar-start">
            <rounter-link to="/" class="navbar-item">Home</rounter-link>
            <rounter-link to="/faq" class="navbar-item">About Us</rounter-link>
            <rounter-link to="/faq" class="navbar-item">Our Client</rounter-link>
            <rounter-link to="/faq" class="navbar-item">Faq</rounter-link>          
          </div>

          <div class="navbar-end">
            <div class="navbar-item">
              <div class="buttons">
                <a class="button is-primary">
                  <strong>Sign up</strong>
                </a>
                <a class="button is-light">
                  Log in
                </a>
              </div>
            </div>
          </div>
        </div>
      </nav>
    </div>
   <router-view></router-view>
   <footer class="footer is-primary ">
     <div class="container">
       <div class="columns">
         <div class="column">
           <p>And this right here is a spiffy footer, where you can put stuff.</p>
         </div>
         <div class="level-right">
           <a class="icon has-text-white" href="#"> <i class="fab fa-facebook"></i></a>
           <a class="icon has-text-white" href="#"> <i class="fab fa-twitter"></i></a>
           <a class="icon has-text-white" href="#"> <i class="fab fa-instagram"></i></a>
           <a class="icon has-text-white" href="#"> <i class="fab fa-youtube"></i></a>
         </div>
       </div>
     </div>
   </footer>
  </div>
</template>

<script>
export default {
  name: 'App',
  data: function(){
    return{
      isActive:false
    }
  },
  methods:{
    toggleNav:function(){
      this.isActive = !this.isActive;
    }
  }
}
</script>

<style lang="sass">

@import '../node_modules/bulma/bulma.sass'
@import 'mq'

.nav
  a:hover
    color: grey


footer
  background-color: $primary !important
  color: #fff

     
</style>
