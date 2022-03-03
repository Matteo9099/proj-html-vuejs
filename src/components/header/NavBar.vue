<template>
    <header>
        <div class="container d-flex align-items-center justify-content-between">
            <!-- Logo -->
            <a href="#">
                <img src="../../assets/img/gym_logo_1x.png" alt="">
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
        background-color: #000;
        z-index: 99;

        a{
            color: #fff;
            font-size: 14px;
            transition: 0.3s;

            &:hover{
                color: $hovMenu;
            }
        }
    }

</style>