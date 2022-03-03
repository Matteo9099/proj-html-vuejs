<template>
    <div class="d-flex text-center" id="jumbotron">
        <!-- testo banner -->
        <div class="container d-flex flex-column justify-content-center align-items-center">
            <h1 class="ms-title-banner text-uppercase text-white">no pain no gain</h1>
            <p class="ms-text-banner">Motivation is what gets you started. Habit is what keeps you going</p>
            <a class="ms-btn px-4 py-2" href="#">Join us today</a>
        </div>


        <!-- Banner img -->
        <div class="d-flex flex-column h-100">
            <!-- <img class="img-fluid" src="../../assets/img/home-banner.jpg" alt="Banner atleta"> -->
        </div>
    </div>
</template>

<script>
export default {
    name: 'MyBanner'
}
</script>

<style lang="scss" scoped>
@import "../../assets/sass/vars.scss";

    #jumbotron{
        background: url('../../assets/img/home-banner.jpg') no-repeat;
        background-position: center;
        background-size: cover;
        height: 100vh;

        .ms-title-banner{
            font-size: 80px;
        }
        .ms-text-banner{
            color: rgb(214, 213, 213);
            font-size: 1.2rem;
        }
        .ms-btn{
            border: 1px solid $colorText;
            text-decoration: none;
            color: $colorText;
            transition: 0.5s;

            &:hover{
                background-color: $hovMenu;
                color: #fff;
            }
        }
    }


</style>