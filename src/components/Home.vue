<template>
  <div>
    <NavBar/>
    <Welcome/>
    <Footer/>
  </div>

</template>

<script>
import NavBar from './Nav.vue'
import Footer from './Footer.vue'
import Welcome from './../views/Welcome.vue'

export default {
  name: 'Home',
    components: {
    NavBar,
    Welcome,
    Footer
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
