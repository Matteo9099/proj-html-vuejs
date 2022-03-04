<template>
    <div>
        <WorldFitness />
        <FormUtente />
        <PointerGym />
        <WorldResult />
        <BannerMain />
        <MeetTrainers />
    </div>
 
</template>

<script>
import WorldFitness from "./main/WorldFitness.vue"
import FormUtente from "./main/FormUtente.vue"
import PointerGym from "./main/PointerGym.vue"
import WorldResult from "./main/WorldResult.vue"
import BannerMain from "./main/BannerMain.vue"
import MeetTrainers from "./main/MeetTrainers.vue"

export default {
    name: 'MyMain',
    components: {
        WorldFitness,
        FormUtente,
        PointerGym,
        WorldResult,
        BannerMain,
        MeetTrainers
    },
}
</script>

<style lang="scss" scoped>

</style>