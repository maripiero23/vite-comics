<template>
    <footer>
        
        <div class="container pt-5">
            <div class="row">
                <div class="col-6">
                    <div class="row d-flex gap-3">
                        <div class="col-3 text-white">
                            <div class="title-footer">
                                <h5 class="fs-semibold text-white">DC COMICS</h5>
                            </div>
                            <ul class="links-footer list-unstyled">
                                <li class="text-secondary"><small>CHARACTERS</small><a href=""></a></li>
                                <li class="text-secondary"><small>COMICS</small><a href=""></a></li>
                                <li class="text-secondary"><small>MOVIES</small><a href=""></a></li>
                                <li class="text-secondary"><small>TV</small><a href=""></a></li>
                                <li class="text-secondary"><small>GAMES</small><a href=""></a></li>
                                <li class="text-secondary"><small>VIDEOS</small><a href=""></a></li>
                                <li class="text-secondary"><small>NEWS</small><a href=""></a></li>
                            </ul>

                            <div class="title-footer">
                                <h5 class="fs-semibold text-white">SHOP</h5>
                            </div>
                            <ul class="links-footer list-unstyled">
                                <li class="text-secondary"><small>SHOP DC</small><a href="">{{link}}</a></li>
                                <li class="text-secondary"><small>SHOP DC Collectibles</small><a href="">{{link}}</a></li>

                            </ul>
                        </div>

                        <div class="col-3 text-white">
                            <div class="title-footer">
                                <h5 class="fs-semibold text-white">DC</h5>
                            </div>
                            <ul class="links-footer list-unstyled">
                                <li class="text-secondary"><small>CHARACTERS</small><a href=""></a></li>
                                <li class="text-secondary"><small>COMICS</small><a href=""></a></li>
                                <li class="text-secondary"><small>MOVIES</small><a href=""></a></li>
                                <li class="text-secondary"><small>TV</small><a href=""></a></li>
                                <li class="text-secondary"><small>GAMES</small><a href=""></a></li>
                                <li class="text-secondary"><small>VIDEOS</small><a href=""></a></li>
                                <li class="text-secondary"><small>NEWS</small><a href=""></a></li>
                                <li class="text-secondary"><small>SHOP DC</small><a href="">{{link}}</a></li>
                                <li class="text-secondary"><small>SHOP DC Collectibles</small><a href="">{{link}}</a></li>
                            </ul>

                        </div>
                        <div class="col-3 text-white">
                            <div class="title-footer">
                                <h5 class="fs-semibold text-white">SITES</h5>
                            </div>
                            <ul class="links-footer list-unstyled">
                                <li class="text-secondary"><small>DC</small><a href=""></a></li>
                                <li class="text-secondary"><small>MAD Magazine</small><a href=""></a></li>
                                <li class="text-secondary"><small>DC Kids</small><a href=""></a></li>
                                <li class="text-secondary"><small>DC Universe</small><a href=""></a></li>
                                <li class="text-secondary"><small>DC Power Visa</small><a href=""></a></li>
    
                            </ul>
                        </div>
                    </div>
    
                </div>
    
                <div class="col-6">
                    <div class="logone">
                        <img src="../assets/img/dc-logo-bg.png" alt="" class="img-big">
                    </div>
    
                </div>
    
            </div>
        </div>
    </footer>
</template>

<script>
export default{
    data(){
        return{
            dcComicsLinks: ['CHARACTERS','COMICS', 'MOVIES', 'TV', 'GAMES', 'VIDEOS', 'NEWS',],
            shopLinks:['SHOP DC', 'SHOP DC Collectibles'],
            dcLinks:['Terms Of Use', 'Privacy policy (New)', 'Ad Choices', 'Advertising', 'Jobs', 'Subscriptions', 'Talent Workshops', 'CPSC Certificates', 'Ratings', 'Shop Help', 'Contact Us'],
            sitesLinks:['DC', 'MAD Magazine', 'DC Kids', 'DC Universe', 'DC Power Visa']


            
            

        
        }
    }
}
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

footer{
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover ;
    position: relative;
}

.logone{
    width: 400px;
    position: absolute;
    top: -42PX;

    .img-big{
        width: 438px;
    }
}

</style>