<template>
    <div class="container d-flex align-items center justify-content-between debug">
        <!-- Logo -->
        <a href="#">
            <img src="../../assets/img/gym_logo_1x.png" alt="">
        </a>
        <!-- Menu -->
        <nav>
            <a 
                v-for="(menuItem, index) in menuItems"
                :key="index"
                href="`#${menuItem.link}`"
                >{{ menuItem.text }}</a
            >  
        </nav>
       
    </div>
</template>

<script>
export default {
    name: 'NavBar',
    props: ["menuItems"],
}
</script>

<style lang="scss" scoped>

    .debug{
        background-color: #000;

        a{
            color: #fff;
        }
    }

</style>