<template>
  <section class="container">
    <div>
    <b-navbar toggleable="" type="dark" variant="info">


      <b-navbar-brand href="#">
        <img class="rounded-circle" src="~assets/logo_perrofeofilms_amarillo.jpg">
      </b-navbar-brand>

    </b-navbar>  


      <div class="youtube" href="#">
            <img src="~assets/youtube.svg">
      </div>
      <div class="email" href="#">
            <img src="~assets/EMAIL.svg">
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
  top: 80px;
  padding: 0 10px;
  
}
.youtube img, .email img{
  width: 30px;
}
.email{
  position: absolute;
  top: 110px;
  left: 15px;
  padding: 10px 10px;
}

@media(max-width:750px) {
    .youtube{
	    position: absolute;
      right: 80px;
      left: 0;
      top: 20px;
      padding: 0 10px;
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

