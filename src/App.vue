<script>
import PageHeader from './components/PageHeader.vue';
import PageMain from './components/PageMain.vue';
import PageFooter from './components/PageFooter.vue';


export default {
  data() {
    return {
      navLinks: [
        {
          href: "#home",
          text: "HOME",
        },
         {
         href: "#pages",
         text: "PAGES",
         },
         {
         href: "#menu",
         text: "MENU",
        },
         {
         href: "#event",
         text: "EVENT",
         },
         {
         href: "#blog",
         text: "BLOG",
         },
         {
         href: "#landing",
         text: "LANDING",
         },
         {
         href: "#cart",
         text: "CART",
         },
         {
         href: "#search",
         text: "SEARCH",
         },
      ],



    }
  },
  components: {
    PageHeader,
    PageMain,
    PageFooter,

  }

}
</script>

<template>
  <header>
    <PageHeader :arrayNav="navLinks" />
  </header>
</template>

<style lang="scss">
@use "./styles/general.scss";
@use "./styles/partials/variables" as *;

header {
  height: 500px;
  background-color: $background-color-first;
  padding-top: 70px;
}

p {
  color: red;
}
</style>
