<template>
  <section class="container">
    <div>
    <b-navbar toggleable="" type="dark" variant="info">


      <b-navbar-brand href="#" v-b-popover.hover="'-Jau!'" title="perrofeofilms">
        <img class="rounded-circle" src="~assets/logo_perrofeofilms_amarillo.jpg" alt="perrofeo logo">
      </b-navbar-brand>

    </b-navbar>  

      <div class="email" v-b-popover.hover="'perrofeofilms@gmail.com'">
            <a href="mailto:perrofeofilms@gmail.com"><img src="~assets/EMAIL.svg" alt="email icon"></a>
      </div>

      <div class="youtube" v-b-popover.hover="'take a look on my YouTube channel!'">
            <a href="https://www.youtube.com/channel/UCWAH8FrQMgxKZYxWPRynrKw" target="_blank" rel="noopener"><img src="~assets/youtube.svg" alt="youtube logo"></a>
      </div>
      <div class="films d-flex justify-content-center">
        <div class="">
        <b-button v-b-popover.hover="'Una historia amazónica protagonizada por Hitler Lomas Canaquiri.'" title="De la selva al mundo">
            <a href="#">La Guitarra de Hitler</a>
        </b-button>
        </div>  
        </div>
     </div>
    
  </section>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  /* align-items: center; */
  text-align: center;
}

.navbar {
  width: 100vw;
}
.navbar img{
  width: 50px;
}

.bg-info {
    background-color: transparent!important;
}

.youtube{
  position: absolute;
  left: 15px;
  top: 120px;
  padding: 0 9px;
  z-index: 3;
  
}
.youtube img{
  width: 32px;
}
.email{
  position: absolute;
  top: 70px;
  left: 15px;
  padding: 10px 10px;
  z-index: 3;
}
.email img{
  width: 30px;
}
.films{
  position: absolute;
  left: 15px;
  top: 175px;
  padding: 0 9px;
  z-index: 3;
}
.films .btn-secondary {
    color: black;
    background-color: #ddfe19;
    border-color: black;
}
.films a{
  color: black;
}
.films a:hover{
  text-decoration: none;
}

@media(max-width:750px) {
    .youtube{
	    position: absolute;
      right: 80px;
      left: 0;
      top: 20px;
      padding: 0 9px;
      text-align: right; 
    }
    .email{
      position: absolute;
      right: 10px;
      left: 0;
      top: 20px;
      text-align: right;
      padding: 0px 10px; 
    }
    .films{
      position: absolute;
   left: auto;
   top: auto;
    bottom: 150px;
    padding: 0 9px;
    z-index: 3;
    /* margin: auto; */
    text-align: center;
    width: 100%;
    }
}
@media(max-width:750px)and (orientation: landscape){
    .films{
      bottom: 80px;
      }
}
</style>
<style scoped>
  section {
    background-image: url("~assets/portada3.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center bottom;
    min-width: 100%;
  }
</style>

