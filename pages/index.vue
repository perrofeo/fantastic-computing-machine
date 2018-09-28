<template>
  <section class="container">
    <div>
    <b-navbar toggleable="" type="dark" variant="info">


      <b-navbar-brand href="#">
        <img class="rounded-circle" src="~assets/logo_perrofeofilms_amarillo.jpg">
      </b-navbar-brand>

    
    <b-navbar-nav>

      <b-nav-item href="#">
            <img src="~assets/youtube.svg">
          </b-nav-item>
      <b-nav-item href="#" right>perrofeofilms@gmail.com</b-nav-item>
    </b-navbar-nav>
    </b-navbar>
    <!-- navbar-1.vue -->
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

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
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

