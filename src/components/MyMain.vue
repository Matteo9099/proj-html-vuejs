<template>
    <div>
        <WorldFitness />
        <FormUtente />
    </div>
 
</template>

<script>
import WorldFitness from "./main/WorldFitness.vue"
import FormUtente from "./main/FormUtente.vue"

export default {
    name: 'MyMain',
    components: {
        WorldFitness,
        FormUtente,
    }
}
</script>

<style lang="scss" scoped>

</style>