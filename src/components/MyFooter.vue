<template>

    <FooterTop :infos="infos"/>

</template>

<script>
import FooterTop from "./footer/FooterTop.vue"

export default {
    name: 'MyFooter',
    components: {
        FooterTop,
    },
    props: ["infos"],
};
</script>

<style>

</style>