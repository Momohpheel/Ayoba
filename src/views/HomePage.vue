<template>
  <div class="body">
    <section id="wrapper" class="">
      <NavBar class="" />
      
      <Products />
      
      
      <!-- <Footer class="footer" /> -->
    </section>
  </div>
</template>
<script>

import Products from "@/components/Main/ExploreProducts"

import NavBar from "@/components/Nav/HomeNavBar"
// import Footer from "@/components/Footer"
export default {
  components: { NavBar, Products},
  created(){
    if(this.$store.state.homeCollapse == true){
      this.$store.commit('setHomeCollapse', false)
    }
  }
  
}
  
</script>


<style scoped>
.body{
  overflow-x: hidden;
  background-color: #FAFAFA;
}
@media only screen and (min-width: 1024px){
  .bigbox{
    max-width: 1024px;
  }
}
@media screen and (min-width: 1280px){
  
}
</style>