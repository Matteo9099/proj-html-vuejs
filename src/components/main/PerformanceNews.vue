<template>
    <section class="py-5">
        <div class="container m-auto text-center">
            <div class="title py-3">
                <h3 class="text-white">PEERFORMANCE NEWS</h3>
                <img src="../../assets/img/divider-xx-red.png" alt="divide-xx">
            </div>
        
            <div class="row m-auto justify-content-center gy-3 text-start">
                <div class="col-3 mx-2 h-100 ms-cardImage mb-3" v-for="(athlete, index) in athletes" :key="index">
                    <img :src="`${athlete.imgUrl}`" class="img-fluid ms-hovImage">
                    <div class="overlay d-flex">
                        <i class="fa-solid fa-link"></i>
                        <i class="fa-solid fa-magnifying-glass"></i>
                    </div>
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

    .ms-cardImage{
        position: relative;
        transition: 0.6s linear;
        padding: 0;
        margin: 0;
        
        &:hover{
            background-color: $hovMenu;
        }
        &:hover img{
            opacity: 0.3;
        }
        &:hover .overlay i{
            display: block;
        }

        .overlay{
            position: absolute;
            top: 25%;
            left: 50%;
            transform: translate(-50%, -50%);
          
            i{
                color:#fff;
                display: none;
                margin-right: 10px;
                font-size: 1.4rem;
                cursor: pointer;
                transition: 0.3s;

                &:hover{
                    transform: scale(1.1);
                }
            }
        }
     
        img {

            display: block;
            width: 100%;
            height: auto;
            transition: .5s ease;
        }
    }


</style>