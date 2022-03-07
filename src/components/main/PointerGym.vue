<template>
    <section class="py-5">
        <div class="container m-auto row py-5">
            <div class="col text-center mx-2" v-for="(menu, index) in menuFitness" :key="index">
                <a href="#">
                    <i :class="menu.icon" class="mb-2"></i>
                </a>
                <h4 class="fw-bold">{{ menu.title }}</h4>
                <img :src="`${menu.img}`" alt="">
                <p>{{ menu.text}}</p>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'PointerGym',
    data() {
        return{
            menuFitness: [
                { 
                    icon:"fa-solid fa-link",
                    title: "Strenght & Conditioning", 
                    img: require("../../assets/img/divider-x-red.png"), 
                    text: "lorem ipsum dolor sit amet, consectetur adipiscing elit. In augue nisl, ornare es volutpat etra us."
                },
                { 
                    icon:"fa-solid fa-bicycle",
                    title: "Strenght & Conditioning", 
                    img: require("../../assets/img/divider-x-red.png"), 
                    text: "lorem ipsum dolor sit amet, consectetur adipiscing elit. In augue nisl, ornare es volutpat etra us."
                },
                { 
                    icon:"fa-solid fa-cloud",
                    title: "Strenght & Conditioning", 
                    img: require("../../assets/img/divider-x-red.png"), 
                    text: "lorem ipsum dolor sit amet, consectetur adipiscing elit. In augue nisl, ornare es volutpat etra us."
                },
                { 
                    icon:"fa-solid fa-heart-pulse",
                    title: "Strenght & Conditioning", 
                    img: require("../../assets/img/divider-x-red.png"), 
                    text: "lorem ipsum dolor sit amet, consectetur adipiscing elit. In augue nisl, ornare es volutpat etra us."
                },
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/sass/vars.scss";

    section{
        background: url("../../assets/img/gym_bkgd_bw-compressor.jpg") no-repeat;
        background-size: cover;
        background-position: center;

        h4{
            color: #fff;
            font-size: 18px
        }
        p{
            color: $colorText;
        }
        i{
            color: $bgLink;
            border: 1px solid $bgLink;
            border-radius: 50%;
            padding: 10px;
            font-size: 1.2rem;
        }

    }

    
</style>