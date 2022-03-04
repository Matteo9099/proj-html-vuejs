<template>
    <section class="py-5">
        <div class="container m-auto text-start">
            <div class="row m-auto justify-content-center gy-3">
                <div class="col-3 mx-2 h-100" v-for="(athlete, index) in athletes" :key="index">
                    <img :src="`${athlete.imgUrl}`" class="img-fluid">
                    <div class="ms-card p-3">
                        <h4 class="text-white">{{ athlete.title }}</h4>
                        <p>{{ athlete.text }}</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'PerformanceNews',
    data(){
        return{
            athletes: [
                {
                    imgUrl: require("../../assets/img/blog1.jpg"), 
                    title: "Train with free weights or your body weight?",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla vel minima maiores. Facere temporibus sequi repudiandae. Aperiam, voluptas accusantium. Sint ipsa fuga perspiciatis quae cum. Cumque doloremque quidem illum fugiat[...]",
                },
                {
                    imgUrl: require("../../assets/img/blog6.jpg"), 
                    title: "Nutritional advice that will keep you training",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla vel minima maiores. Facere temporibus sequi repudiandae. Aperiam, voluptas accusantium. Sint ipsa fuga perspiciatis quae cum. Cumque doloremque quidem illum fugiat[...]",
                },
                {
                    imgUrl: require("../../assets/img/trainer4.jpg"), 
                    title: "Simple principles for your next workout",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla vel minima maiores. Facere temporibus sequi repudiandae. Aperiam, voluptas accusantium. Sint ipsa fuga perspiciatis quae cum. Cumque doloremque quidem illum fugiat[...]",
                },
                {
                    imgUrl: require("../../assets/img/blog4.jpg"), 
                    title: "To be number one, train like you're number two",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla vel minima maiores. Facere temporibus sequi repudiandae. Aperiam, voluptas accusantium. Sint ipsa fuga perspiciatis quae cum. Cumque doloremque quidem illum fugiat[...]",
                },
                {
                    imgUrl: require("../../assets/img/trainer3.jpg"), 
                    title: "Top 5 mistakes every gym member makes",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla vel minima maiores. Facere temporibus sequi repudiandae. Aperiam, voluptas accusantium. Sint ipsa fuga perspiciatis quae cum. Cumque doloremque quidem illum fugiat[...]",
                },
                {
                    imgUrl: require("../../assets/img/trainer1.jpg"),
                    title: "The myths of shedding body fat explored",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla vel minima maiores. Facere temporibus sequi repudiandae. Aperiam, voluptas accusantium. Sint ipsa fuga perspiciatis quae cum. Cumque doloremque quidem illum fugiat[...]",
                },
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/sass/vars.scss";

    section{
        background-color: $bgBanner;

        .ms-card{
            background-color: $bgBannerDue;

            h4{
                font-size: 0.9rem;
            }
            p{
                color: $colorText;
                font-size: 0.9rem;
            }
        }
    }

</style>