<template>
    <section class="py-5">
        <!-- Real World Result -->
        <div class="container m-auto pb-5">
            <div class="row g-4">
                <div class="col-12 text-center">
                    <h4>REAL WORLD RESULTS</h4>
                    <img src="../../assets/img/divider-xx-red.png" class="py-3" alt="img x">
                </div>
                <div class="col-6 d-flex" v-for="(list, index) in listResults" :key="index">
                    <div class="row ms-card p-3 mx-3">
                        <div class="col-4">
                            <img :src="`${list.imgUrl}`" alt="img testimone">
                        </div>
                        <div class="col-8 d-flex flex-column">
                            <cite>{{ list.text }}</cite>
                            <span class="mt-2">{{ list.author }}</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <!-- Hight performance facilities -->
        <div class="container m-auto pt-5">
            <div class="row g-4">
                <div class="col-12 text-center">
                    <h4>HIGHT PERFORMANCE FACILITIES</h4>
                    <img src="../../assets/img/divider-xx-red.png" class="py-3" alt="img x">
                </div>      
                <div class="col-4 d-flex" v-for="(image, index) in imageLists" :key="index">
                    <img :src="`${image.img}`" alt="">
                </div>          
            </div>

        </div>
    </section>
</template>

<script>
export default {
    name: 'WorldResult',
    data(){
        return{
            listResults:[
                { 
                    imgUrl: require("../../assets/img/review_1-compressor.jpg"), 
                    text: "The trainers at Avada Gym have helped me reach my fitness goals beyond anything I could of hoped for. I love it!", 
                    author: "- Tara Smith" 
                },
                { 
                    imgUrl: require("../../assets/img/review_3-compressor-2.jpg"), 
                    text: "The atmosphere at Avada Gym is amazing, the people are even better. All in all, it is a great place to work out.", 
                    author: "- Simon Chel" 
                },
                { 
                    imgUrl: require("../../assets/img/review_2-compressor.jpg"), 
                    text: "The facilities at Avada Gym stood out to me the most. They are well maintained and have high quality equipment.", 
                    author: "- Jen Wirth" 
                },
                { 
                    imgUrl: require("../../assets/img/review_4-compressor-2.jpg"), 
                    text: "Not bad things to say about Avada Gym, they are top notch at every corner and truly take care of thei customers.", 
                    author: "- Jeff Glum" 
                },
            ],
            imageLists:[
                { img: require("../../assets/img/home-image1.jpg") },
                { img: require("../../assets/img/home-image2.jpg") },
                { img: require("../../assets/img/home-image3.jpg") },
                { img: require("../../assets/img/home-image4.jpg") },
                { img: require("../../assets/img/home-image54.jpg") },
                { img: require("../../assets/img/home-image6.jpg") },
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/sass/vars.scss";

    section{
        background-color: $bgBanner;
        color: #fff;

        .ms-card{
            background: $bgBannerDue;

            cite{
                color: $colorText;
            }
            span{
                color: rgb(209, 206, 206);
            }
        }
    }

</style>