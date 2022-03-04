<template>
    <div>
        <FooterTop :infos="infos" />
        <FooterBottom :linkBottom="linkBottom" />
    </div>
    

</template>

<script>
import FooterTop from "./footer/FooterTop.vue"
import FooterBottom from "./footer/FooterBottom.vue"

export default {
    name: 'MyFooter',
    components: {
        FooterTop,
        FooterBottom,
    },
    props: ["infos", "linkBottom"],
};
</script>

<style>

</style>