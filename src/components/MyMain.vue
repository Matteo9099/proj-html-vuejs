<template>
    <div>
        <WorldFitness />
        <FormUtente />
        <PointerGym />
        <WorldResult />
        <BannerMain />
    </div>
 
</template>

<script>
import WorldFitness from "./main/WorldFitness.vue"
import FormUtente from "./main/FormUtente.vue"
import PointerGym from "./main/PointerGym.vue"
import WorldResult from "./main/WorldResult.vue"
import BannerMain from "./main/BannerMain.vue"

export default {
    name: 'MyMain',
    components: {
        WorldFitness,
        FormUtente,
        PointerGym,
        WorldResult,
        BannerMain,
    },
}
</script>

<style lang="scss" scoped>

</style>