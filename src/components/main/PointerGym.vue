<template>
    <section class="py-5">
        <div class="container m-auto row py-5">
            <div class="col text-center mx-2" v-for="(menu, index) in menuFitness" :key="index">
                <h5 class="fw-bold">{{ menu.title }}</h5>
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
                    title: "Strenght & Conditioning", 
                    img: require("../../assets/img/divider-x-red.png"), 
                    text: "lorem ipsum dolor sit amet, consectetur adipiscing elit. In augue nisl, ornare es volutpat etra us."
                },
                { 
                    title: "Strenght & Conditioning", 
                    img: require("../../assets/img/divider-x-red.png"), 
                    text: "lorem ipsum dolor sit amet, consectetur adipiscing elit. In augue nisl, ornare es volutpat etra us."
                },
                { 
                    title: "Strenght & Conditioning", 
                    img: require("../../assets/img/divider-x-red.png"), 
                    text: "lorem ipsum dolor sit amet, consectetur adipiscing elit. In augue nisl, ornare es volutpat etra us."
                },
                { 
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

        h5{
            color: #fff;
        }
        p{
            color: $colorText;
        }

    }

    
</style>