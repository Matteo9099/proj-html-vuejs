<template>
    <div>
        <FitnessGoals />
        <FooterTop :infos="infos" />
        <FooterBottom :linkBottom="linkBottom" />
    </div>
    

</template>

<script>
import FooterTop from "./footer/FooterTop.vue"
import FooterBottom from "./footer/FooterBottom.vue"
import FitnessGoals from "./footer/FitnessGoals.vue"

export default {
    name: 'MyFooter',
    components: {
        FooterTop,
        FooterBottom,
        FitnessGoals,
    },
    props: ["infos", "linkBottom"],
};
</script>

<style>

</style>