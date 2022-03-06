<template>
    <section class="py-3">
        <div class="container">
            <div class="row justify-content-between align-items-center">
                <div class="col">
                    <ul class=" d-flex">
                        <li class="nav-item d-flex" v-for="(link, index) in linkBottom" :key="index">
                            <a class="nav-link" :href="link.link">{{ link.text }}</a>
                        </li>
                    </ul>
                </div>
             
                <div class="col">
                    <a href="#" v-for="(social, index) in linkBottom" :key="index">
                        <i :class="social.icon"></i>
                    </a>
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
            background-color: $bgLink;
        }
    }
   

</style>