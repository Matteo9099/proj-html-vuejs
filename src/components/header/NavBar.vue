<template>
    <header>
        <div class="container d-flex align-items-center justify-content-between ms-brand">
            <!-- Logo -->
            <a href="#">
                <img  src="../../assets/img/gym_logo_1x.png" alt="">
            </a>
            <!-- Menu -->
            <nav>
                <ul class="navbar-nav">
                    <li class="nav-item d-flex">
                        <a 
                            class="nav-link mx-3 text-uppercase"
                            v-for="(menuItem, index) in menuItems"
                            :key="index"
                            href="`#${menuItem.link}`"
                            >{{ menuItem.text }}</a
                        >  
                    </li>
                </ul>
            </nav>
        </div>
    </header>
   
</template>

<script>
export default {
    name: 'NavBar',
    props: ["menuItems"],
}
</script>

<style lang="scss" scoped>
@import "../../assets/sass/vars.scss";

    header{
        position: fixed;
        width: 100%;
        background-color: rgba($color: #000000, $alpha: 0.9);
        z-index: 99;

        .ms-brand{
            height: 100px;

            img{
                height: 100%;
            }
        }

        a{
            color: #fff;
            font-size: 14px;
            transition: 0.3s;
            height: 100%;

            &:hover{
                color: $hovMenu;
            }
        }
    }

</style>