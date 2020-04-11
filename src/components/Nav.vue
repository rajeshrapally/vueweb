<template>
    <div>
        <b-navbar toggleable="lg" type="dark" variant="info">
    <b-navbar-brand href="#">{{site_title}}</b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>


      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">

        <b-navbar-nav>
            <router-link to="/foo">Go to Foo</router-link>
            <b-nav-item v-for="(item,index) in menuitems" :key="index">{{item}}</b-nav-item>
        </b-navbar-nav>
        
        <b-nav-form right>
          <b-form-input size="sm" class="mr-sm-2" placeholder="Search"></b-form-input>
          <b-button size="sm" class="my-2 my-sm-0" type="submit">Search</b-button>
        </b-nav-form>
 
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
    </div>
</template>

<script>
    export default {
        name: "NavBar",
        data() {
            return {
                site_title: "VueWeb Site",
                menuitems: ["Home","about","contact"]
            }            
        }
    }
</script>

<style lang="scss" scoped>

</style>