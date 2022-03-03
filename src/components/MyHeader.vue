<template>
    <div>
        <NavBar />

    </div>

</template>

<script>
import NavBar from "./header/NavBar.vue"


export default {
    name: 'MyHeader',
    components: {
        NavBar,
    },
    props: ["menuItems"],
};
</script>

<style>

</style>