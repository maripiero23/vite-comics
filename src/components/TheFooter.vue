<template>
    <footer>
        
        <div class="container pt-5">
            <div class="row">
                <div class="col-6">
                    <div class="row">
                        <div class="col-4 text-white">
                            <div>DC COMICS</div>
                            <div>hhhh</div>
                            <div>hhhh</div>
                            <div>hhhh</div>
                            <div>hhhh</div>
                            <div>hhhh</div>
    
                            
                        </div>
                        <div class="col-4 text-white">
                            <div>DC COMICS</div>
                            <ul>
                                <li>link</li>
                                <li>link</li>
                                <li>link</li>
                                <li>link</li>
                                <li>link</li>
    
                            </ul>
                        </div>
                        <div class="col-4 text-white">
                            <div>DC COMICS</div>
                            <ul>
                                <li>link</li>
                                <li>link</li>
                                <li>link</li>
                                <li>link</li>
                                <li>link</li>
    
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

        }
    }
}
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

footer{
    background-image: url(../assets/img/footer-bg.jpg);
    padding: 3rem 0;
    position: relative;
}

.logone{
    width: 400px;
    position: absolute;
    top: -20px;

    .img-big{
        width: 400px;
    }
}

</style>