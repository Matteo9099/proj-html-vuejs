<template>
    <div>
        <NavBar :menuItems="menuItems"/>
        <MyBanner />
    </div>

</template>

<script>
import NavBar from "./header/NavBar.vue"
import MyBanner from "./header/MyBanner.vue"


export default {
    name: 'MyHeader',
    components: {
        NavBar,
        MyBanner,
    },
    props: ["menuItems"],
};
</script>

<style>

</style>