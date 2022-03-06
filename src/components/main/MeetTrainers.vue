<template>
  <section class="py-5 text-center">
        <div class="container row m-auto d-flex justify-content-center">
            <div class="title py-4">
                <h3 class="text-white">MEET OUR TRAINERS</h3>
                <img src="../../assets/img/divider-xx-red.png" alt="divider xx">
            </div>
            
            <!-- 
            <div class="col-3 d-flex flex-column mx-2" v-for="(trainer, index) in listTrainers" :key="index">
                <img class="w-100" :src="`${trainer.imgUrl}`" alt="">
                <div class="container d-flex flex-column text-start pt-3 ms-bgCard mb-5">
                    <span class="text-white fw-bold">{{ trainer.name }}</span>
                    <span class="text-white fw-bold">{{ trainer.profession }}</span>
                    <p class="my-3">{{ trainer.text }}</p>   
                    <div class="socials d-flex py-4">
                        Icone social
                        <div v-for="(social,index) in trainer.socials" :key="trainer.name + index">
                            <a :href="social.url" class=" py-2 px-3 rounded me-3">
                                <i :class="social.icon"></i>
                            </a>
                        </div>
                    </div>
                </div>
            </div> 
            -->


            <div class="container">
                <div class="ms-card" v-for="(trainer, index) in listTrainers" :key="index">
                    <div class="face face1">
                        <div class="content">
                            <img :src="`${trainer.imgUrl}`" alt="">
                        </div>
                    </div>
                    <div class="face face2 d-flex flex-column">
                        <div class="content">
                            <h4 class="text-white fw-bold">{{ trainer.name }}</h4>
                            <span class="text-white fw-bold">{{ trainer.profession }}</span>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime ipsum ab est dicta omnis dolor, autem adipisci.</p>

                            <div class="d-flex">
                                <ul class="d-flex">
                                    <li class="nav-item" v-for="(social,index) in trainer.socials" :key="trainer.name + index">
                                        <a :href="social.url" class=" py-2 px-3 rounded me-3">
                                            <i :class="social.icon"></i>
                                        </a>
                                    </li>
                                </ul>
                               
                            </div>

                        </div>
                        
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
                    socials: [
                        { 
                            icon: "fa-brands fa-facebook-f", url:"#" 
                        },
                        { 
                            icon: "fa-brands fa-twitter", url:"#" 
                        },
                        { 
                            icon: "fa-brands fa-instagram", url:"#" 
                        },
                    ],
                    imgUrl: require("../../assets/img/trainer1.jpg"),
                    name: "Ann Baker",
                    profession: "Personal Trainer",
                    text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. In augue nisl, onare volutpat."
                },
                {
                    socials: [
                        { 
                            icon: "fa-brands fa-facebook-f", url:"#" 
                        },
                        { 
                            icon: "fa-brands fa-twitter", url:"#" 
                        },
                        { 
                            icon: "fa-brands fa-instagram", url:"#" 
                        },
                    ],
                    imgUrl: require("../../assets/img/trainer3.jpg"),
                    name: "Anne Warren",
                    profession: "Personal Trainer",
                    text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. In augue nisl, onare volutpat."
                },
                {
                    socials: [
                        { 
                            icon: "fa-brands fa-facebook-f", url:"#" 
                        },
                        { 
                            icon: "fa-brands fa-twitter", url:"#" 
                        },
                        { 
                            icon: "fa-brands fa-instagram", url:"#" 
                        },
                    ],
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
        a{
            color: #fff;
            background-color: $bgBannerDue;
        }
    }




    .container{
        width: 1000px;
        position: relative;
        display: flex;
        justify-content: space-between;
    }

    .container .ms-card{
        position: relative;
        cursor: pointer;
    }

    .container .ms-card .face{
        width: 300px;
        height: 200px;
        transition: 0.5s;
    }

    .container .ms-card .face.face1{
        position: relative;
        background: #333;
        display: flex;
        justify-content: center;
        align-items: center;
        z-index: 1;
        transform: translateY(100px);
    }

    .container .ms-card:hover .face.face1{
        background: #ff0057;
        transform: translateY(0);
    }

    .container .ms-card .face.face1 .content{
        transition: 0.5s;
    }

    .container .ms-card:hover .face.face1 .content{
        opacity: 1;
    }

    .container .ms-card .face.face1 .content img{
        width: 100%;
    }

    .container .ms-card .face.face2 .content h4{
        margin-top: 25px;
        padding: 0;
        color: #fff;
        text-align: center;
        font-size: 1.5rem;
    }

    .container .ms-card .face.face2{
        position: relative;
        background: $bgBanner;
        display: flex;
        justify-content: center;
        align-items: center;
        padding: 20px;
        box-sizing: border-box;
        box-shadow: 0 20px 50px rgba(0, 0, 0, 0.8);
        transform: translateY(-100px);
    }

    .container .ms-card:hover .face.face2{
        transform: translateY(0);
    }

    .container .ms-card .face.face2 .content p{
        margin: 0;
        padding: 0;
    }

    .container .ms-card .face.face2 .content a{
        margin: 15px 0 0;
        display: inline-block;
        text-decoration: none;
        font-weight: 900;
        color: #333;
        padding: 5px;
        border: 1px solid #333;
    }

    .container .ms-card .face.face2 .content a:hover{
        background: #333;
        color: #fff;
    }



</style>