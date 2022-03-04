<template>
    <section class="py-5">
        <div class="container row m-auto">
            <div class="col">
                <img src="../../assets/img/home_img-compressor.jpg" alt="atleti uomo donna">
            </div>
            <div class="col">
                <h3>Sign Up For A Free Training Session!</h3>
                <form class="d-flex flex-column">
                    <span>Nome*</span>
                    <input type="text" class="form-control">
                    <span class="mt-3">Email</span>
                    <input type="text" class="form-control">
                    <button class="btn rounded-0 mt-4 text-uppercase">start now!</button>
                </form>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'FormUtente',
}
</script>

<style lang="scss" scoped>
@import "../../assets/sass/vars.scss";

    section{
        background-color: $bgBannerDue;

        img{
            width: 420px;
        }
        h3{
            color: #fff;
        }
        span{
            color: $colorText;
        }
        input{
            background-color: $bgBannerDue;
        }
        button{
            background-color: $hovMenu;
            color: #fff;
            transition: 0.5s;

            &:hover{
                color: #fff;
                transform: scale(0.98);
            }
        }
    }

    

</style>