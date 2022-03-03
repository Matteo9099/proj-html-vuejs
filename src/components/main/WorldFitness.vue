<template>
  <section class="d-flex justify-content-center align-item-center py-5">
        <div class="title-text text-center w-50">
            <h2 class="text-white">WORLD CLASS Fitness</h2>
            <img src="../../assets/img/divider-xx-red.png" class="py-4" alt="img x">
            <p>At Avada Gym, everything we do from top to bottom is of the highest quality to ensure we're equipped to help you reach goals of a healthy and fit lifestyle.</p>
        </div>
  </section>
</template>

<script>
export default {
    name: 'WorldFitness'
}
</script>

<style lang="scss" scoped>
@import "../../assets/sass/vars.scss";

    section{
        background-color: $bgBanner;
        border-bottom: 1px solid red;

        p{
            color: $colorText;
        }
    }

</style>