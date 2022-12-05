<template>
   <div class="banner-container">
        <!-- v-for="(brands, i) in brandList" :key="i + brands.text"  provato ma non viene -->
    <div class="brand-container">  
        <div class="logo">
            <img class="brand-img" src="../assets/img/buy-comics-digital-comics.png" alt="">
        </div>
        <div class="btand-text ps-3">
            <div>DIGITAL COMICS</div>
        </div>
    </div>

    <div class="brand-container">  
        <div class="logo">
            <img class="brand-img" src="../assets/img/buy-comics-merchandise.png" alt="">
        </div>
        <div class="btand-text ps-3">
            <div>DC MERCHANDISE</div>
        </div>
    </div>

    <div class="brand-container">  
        <div class="logo">
            <img class="brand-img" src="../assets/img/buy-comics-subscriptions.png" alt="">
        </div>
        <div class="btand-text ps-3">
            <div>DC SUBSCRIPTION</div>
        </div>
    </div>

    <div class="brand-container">  
        <div class="logo">
            <img class="brand-img" src="../assets/img/buy-comics-shop-locator.png" alt="">
        </div>
        <div class="btand-text ps-3">
            <div>COMIC SHOP LOCATOR</div>
        </div>
    </div>

    <div class="brand-container">  
        <div class="logo">
            <img class="brand-img" src="../assets/img/buy-dc-power-visa.svg" alt="">
        </div>
        <div class="btand-text ps-3">
            <div>DC POWER VISA</div>
        </div>
    </div>

    


   </div>
</template>



<script>
export default{
    data(){
        return{
            brandList:[
                {
                    img: 'buy-comics-digital-comics.png',
                    text: 'DIGITAL COMICS',
                },

                {
                    img:'buy-comics-merchandise.png',
                    text: 'DC MERCHANDISE',
                },

                {
                    img:'buy-comics-subscriptions.png',
                    text:'SUBSCRIPTION',
                },

                {
                    img: 'buy-comics-shop-locator.png',
                    text: 'COMIC SHOP LOCATOR',
                },

                {
                    img: 'buy-dc-power-visa.svg',
                    text: 'DC POWER VISA'
                },

                
            ]
        }
    }
}


</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

.banner-container{
    @include flex_just_center;
    background-color: $banner-color;
    align-items: center;
    padding: 2rem;
    

    .brand-container{
        display: flex;
    }

    .btand-text{
        display: flex;
        align-items: center;
        color: $color-secondary-text;
        }
}

.brand-img{
    width: 30px;
    height: 30px;
    object-fit: contain;
}
</style>