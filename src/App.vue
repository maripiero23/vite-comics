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

      cardsList: [
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
    "price": "$19.99",
    "series": "Action Comics",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
    "price": "$3.99",
    "series": "American Vampire 1976",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
    "price": "$16.99",
    "series": "Aquaman",
    "type": "graphic novel"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
    "price": "$2.99",
    "series": "Batgirl",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
    "price": "$3.99",
    "series": "Batman",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
    "price": "$2.99",
    "series": "Batman Beyond",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
    "price": "$3.99",
    "series": "Batman/Superman",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
    "price": "$4.99",
    "series": "Batman/Superman Annual",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
    "price": "$5.99",
    "series": "Batman: The Joker War Zone",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
    "price": "$6.99",
    "series": "Batman: Three Jokers",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
    "price": "$4.99",
    "series": "Batman: White Knight Presents: Harley Quinn",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
    "price": "$16.99",
    "series": "Catwoman",
    "type": "graphic novel"
  }
]

    }
  }
}

</script>

<template>


  <TheHeader></TheHeader>
  <main>
  
    <img class="img-jumb" src="./assets/img/jumbotron.jpg" alt="">
    
    <div class="container py-5">
      <div class="current-series-container bg-primary">
        <span>CURRENT SERIES</span>
      </div>

      <div class="cards-container">
        <div class="row row-cols-1 row-cols-md-6 g-4">

          <!-- Singola Card -->
          <div class="col" v-for="(card, i) in cardsList" :key="('carta_' + i)">
            <div class="card d-flex">
              <img :src="card.thumb" class="card-img-top" alt="...">
              
              <div class="card-body">
                <h5 class="card-title">{{card.series}}</h5>
                <p>Tipologia: {{card.type}}</p>
                <span>Prezzo: {{card.price}}</span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="button-container d-flex justify-content-center pb-3">
      <button type="button" class="btn btn-primary fw-semibold rounded-0 px-5">LOAD MORE</button>
    </div>

  </main>  
  <TheMain></TheMain>
  
  <BannerOne></BannerOne>
  
  
  <TheFooter></TheFooter>
  
  <BannerTwo></BannerTwo>

    
</template>

<!-- carico il file general.scss -->
<style lang="scss" >
@use './styles/general.scss' as *;

  main{
    background-color: rgba(28,28,28,255);
    
  }

  .current-series-container{
    width: 150px;
    display: flex;
    justify-content: center;
    color: white;
    font-weight: 500;
    position: relative;
    top: -66px;
    padding: 5px;
  }

  .img-jumb{
    width: 100%;
    height: 25rem;

  }

  .card{
    border: none;
    background-color: rgba(28,28,28,255);
    color: white;

  }

  

</style>
