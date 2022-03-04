<template>
    <section class="py-3">
        <div class="container d-flex justify-content-between align-items-center">
            <div class="links">
                <div class="row">
                    <div class="col" v-for="(link, index) in linkBottom" :key="index">
                        <ul class="navbar-nav">
                            <li class="nav-item d-flex">
                                <a class="nav-link" href="`#${link.link}`">{{ link.text }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="socials">

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

         li{
            width: 180px;
        }
        a{
            font-size: 0.8rem;
            color: $colorText;

            &:hover{
                text-decoration: underline;
                color: $colorText;
            }
        }
    }
   

</style>