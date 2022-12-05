<template>
    
    <section class="sign-icons-section">
        <div class="container butt-icons-flex">
            <div class="sign-up">
                <button type="button" class="btn btn-outline-primary rounded-0 text-white px-2 fw-semibold">SIGN-UP NOW!</button>
            </div>
        
            <div class="follow-icons-container">
                <span class="text-primary fw-semibold">FOLLOW US</span>
                <img class="icons" src="" alt="">
                <img class="icons" src="../assets/img/footer-facebook.png" alt="">
                <img class="icons" src="../assets/img/footer-youtube.png" alt="">
                <img class="icons" src="../assets/img/footer-pinterest.png" alt="">
                <img class="icons" src="../assets/img/footer-periscope.png" alt="">

            </div>
        </div>

        
    </section>

</template>

<script>
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

.sign-icons-section{
    @include flex_align_center;
    background-color: rgba(48,48,48,255);
    position: relative;

    .butt-icons-flex{
        @include flex_space_between;
        align-items: center;
    }
}

.icons{
    width: 56px;
    padding-left: 2rem;
}



</style>