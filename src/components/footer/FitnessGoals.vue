<template>
    <section class="py-5">
        <div class="container row m-auto d-flex align-items-center">
            <div class="col-6">
                <h2 class="text-white">Achieve You Fitness Goals</h2>
                <p class="text-white">Flexible membership packages to suit all levels of athlete and achive your fitness goals</p>
            </div>
            <div class="col-3 offset-3">
                <a class="px-4 py-2" href="#">Join us</a>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'FitnessGoals',
}
</script>

<style lang="scss" scoped>
@import "../../assets/sass/vars.scss";

    section{
        background: url('../../assets/img/home-parallax.jpg') no-repeat;
        background-size: cover;
        background-position: center;

        a{  
            border: 1px solid rgb(202, 202, 202);
            color: rgb(202, 202, 202);
            text-decoration: none;
            transition: 0.5s;

            &:hover{
                box-shadow: 200px 0 #fff inset;
                color: $bgLink;
            }
        }
    }

</style>