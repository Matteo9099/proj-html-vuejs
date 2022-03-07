<template>
    <section class="py-3">
        <div class="container">
            <div class="row justify-content-between align-items-center">
                <div class="col">
                    <ul class=" d-flex">
                        <li class="nav-item d-flex ms-4" v-for="(link, index) in linkBottom" :key="index">
                            <a class="nav-link" :href="link.link">
                                {{ link.text }}
                            </a>
                            <a href="#" v-for="(social, index) in link.socials" :key="index">
                                <i :class="social.icon" class="py-2 px-3 mx-2"></i>
                            </a>
                        </li>
                    </ul>
                    <div class="col">
                       
                    </div>
                </div>
             
                
            
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'FooterBottom',
    props: ["linkBottom"],
}
</script>

<style lang="scss" scoped>
@import "../../assets/sass/vars.scss";

    section{
        background-color: $bgBannerDue;

        a{
            font-size: 0.8rem;
            color: $colorText;

            &:hover{
                text-decoration: underline;
                color: $colorText;
            }
        }
        i{
            background-color: $hovMenu;
            font-size: 1.1rem;
        }
    }


</style>