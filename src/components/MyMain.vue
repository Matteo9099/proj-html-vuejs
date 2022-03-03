<template>
    <div>
        <WorldFitness />
        <FormUtente />
        <PointerGym />
    </div>
 
</template>

<script>
import WorldFitness from "./main/WorldFitness.vue"
import FormUtente from "./main/FormUtente.vue"
import PointerGym from "./main/PointerGym.vue"

export default {
    name: 'MyMain',
    components: {
        WorldFitness,
        FormUtente,
        PointerGym,
    },
}
</script>

<style lang="scss" scoped>

</style>