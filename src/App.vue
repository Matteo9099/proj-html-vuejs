<template>
  <div id="app">
      <MyHeader :menuItems="menuItems"/>
  </div>
</template>

<script>
import MyHeader from "./components/MyHeader.vue"

export default {
  name: 'App',
  components: {
    MyHeader,
  },
  data() {
    return{
      menuItems: [
        { text: "Home", link: "home" },
        { text: "About us", link: "about-us" },
        { text: "Facilities", link: "Facilities" },
        { text: "Membership", link: "Membership" },
        { text: "Testimonials", link: "Testimonials" },
        { text: "Blog", link: "Blog" },
      ],
    }
  }
}
</script>

<style lang="scss">
@import "./assets/sass/style.scss";

</style>
