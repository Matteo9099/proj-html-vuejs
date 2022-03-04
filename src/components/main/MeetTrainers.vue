<template>
  <section class="py-5 text-center">
        <div class="container row m-auto d-flex justify-content-center">
            <div class="title py-4">
                <h3 class="text-white">MEET OUR TRAINERS</h3>
                <img src="../../assets/img/divider-xx-red.png" alt="divider xx">
            </div>
            <div class="col-3 d-flex flex-column mx-2" v-for="(trainer, index) in listTrainers" :key="index">
                <img class="w-100" :src="`${trainer.imgUrl}`" alt="">
                <div class="container d-flex flex-column text-start pt-3 ms-bgCard mb-5">
                    <span class="text-white fw-bold">{{ trainer.name }}</span>
                    <span class="text-white fw-bold">{{ trainer.profession }}</span>
                    <p class="my-3">{{ trainer.text }}</p>   
                    <div class="socials d-flex">
                        <!-- Icone social -->
                    </div>
                </div>
            </div>
        </div>
        <a class="ms-btn px-4 py-2 text-center mt-5" href="#">VIEW ALL TRAINERS</a>
  </section>
</template>

<script>
export default {
    name: 'MeetTrainers',
    data(){
        return{
            listTrainers:[
                {
                    imgUrl: require("../../assets/img/trainer1.jpg"),
                    name: "Ann Baker",
                    profession: "Personal Trainer",
                    text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. In augue nisl, onare volutpat."
                },
                {
                    imgUrl: require("../../assets/img/trainer3.jpg"),
                    name: "Anne Warren",
                    profession: "Personal Trainer",
                    text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. In augue nisl, onare volutpat."
                },
                {
                    imgUrl: require("../../assets/img/trainer4.jpg"),
                    name: "Peter Rice",
                    profession: "Personal Trainer",
                    text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. In augue nisl, onare volutpat."
                },
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/sass/vars.scss";

    section{
        background-color: $bgBannerDue;

        .ms-bgCard{
            background-color: $bgBanner;
        }
        span{
            font-size: 0.9rem;
        }
        p{
            color: $colorText;
            font-size: 0.9rem;
        }
        .ms-btn{
            border: 1px solid $colorText;
            text-decoration: none;
            color: $colorText;
        }
    }


</style>