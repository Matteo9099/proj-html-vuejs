<template>
  <section>
      <div class="container">
          <div class="row py-5">
              <div class="col" v-for="(info, index) in infos" :key="index">
                  <!-- titolo link -->
                  <h5 class="fw-bold pb-4">{{ info.title }}</h5>
                  <!-- link -->
                  <ul class="navbar-nav">
                      <li class="nav-item" v-for="(text, index) in info.texts" :key="index">
                          <a class="nav-link" href="#">{{ text }}</a>
                      </li>
                  </ul>
              </div>
              <div class="col">
                  <img src="../../assets/img/gym_ad-compressor.jpg" alt="coupon">
              </div>
          </div>
      </div>
  </section>
</template>

<script>
export default {
    name: 'FooterTop',
   props: ["infos", "footerCoupon"],
}
</script>

<style lang="scss" scoped>
@import "../../assets/sass/vars.scss";

   section{
       background-color: $bgBanner;

       h5{
           color: #7e8995;
       }
       a{
           color: $colorText;

           &:hover{
               text-decoration: underline;
                color: $colorText;
           }
       }
    
   }

</style>