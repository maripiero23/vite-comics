<template>
    <nav class="my-navbar ">  
        <div class="logo">
                <img src="/dc-logo.png" class="img-fluid" alt="">
        </div>

        <ul>
                <li v-for="link in linkList"><a href="#" class="fw-bolder fs-sm"><small>{{link}}</small></a></li>
                             
        </ul>
    </nav>
    <!-- d-flex justify-content-between -->
</template>

<script>
export default{
    data() {
        return{
            linkList: ["CHARACTERS", "COMICS", "MOVIES", "TV", "GAMES", "COLLECTIBLES", "VIDEOS", "FANS", "NEWS","SHOP"],

        }
    }
}
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

.my-navbar{
    @include flex_space_around; 
    padding: 2rem;

    img{
        width: 80px;
    }

    ul{
        list-style: none;
        @include flex_just_center;
        align-items: center;
        font-size: 14px;

        a{
            padding: 1rem ;
            text-decoration: none;
            color: $color_text;
        }
    }
}


</style>