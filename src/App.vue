<script>
import TheHeader from './components/TheHeader.vue'
import TheMain from './components/TheMain.vue'
import TheFooter from './components/TheFooter.vue'
import BannerTwo from './components/BannerTwo.vue'
import BannerOne from './components/BannerOne.vue'


export default{
  components: {TheHeader, TheFooter, TheMain, BannerOne, BannerTwo},
  data() {
    return{

    }
  }
}

</script>

<template>
  <body>
    <div class="container">
      <TheHeader></TheHeader>
    
      <TheMain></TheMain>
    
      <BannerOne></BannerOne>
    
    
      <Footer></Footer>
    
      <BannerTwo></BannerTwo>
  
    </div>
    
  </body>




  
    
</template>

<!-- carico il file general.scss -->
<style lang="scss" >
@use './styles/general.scss'

</style>
