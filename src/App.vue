<template>
  <div id="app">
      <MyHeader :menuItems="menuItems" />
      <MyMain />
      <MyFooter :infos="infos" :linkBottom="linkBottom" />
  </div>
</template>

<script>
import MyHeader from "./components/MyHeader.vue"
import MyFooter from "./components/MyFooter.vue"
import MyMain from "./components/MyMain.vue"

export default {
  name: 'App',
  components: {
    MyHeader,
    MyFooter,
    MyMain,
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
      // footer nav
      infos: [
        // link nav 1
        {
          title: "COME FIND US",
          texts: [
              "12345 North Main Street",
              "New York, NY 55555",
              "Phone: 1.800.555.6789",
              "Email: info@your-domain.com"
          ],
        },
        // link nav 2
        {
          title: "RECENT POSTS",
          texts: [
              "Train with free weights or your body weight?",
              "Nutritional advice that will keep you training",
          ],
        },
        // link nav 3
        {
          title: "OPENING TIMES",
          texts: [
              "Weekdays Monday - Friday",
              "9:00 - 19:00",
              "Weekdays Saturday - Sunday",
              "9:00 - 21:00"
          ],
        },
      ],
      linkBottom:[
        { text: "Copyright 2012 - 2020", link: "copyright" },
        { text: "Avada Theme by Theme Fusion", link: "avada-theme" },
        { text: "All Rights Reserved", link: "reserved" },
        { text: "Powered by WordPress", link: "wordPress" },
      ],
    }
  }
}
</script>

<style lang="scss">
@import "./assets/sass/style.scss";


</style>
