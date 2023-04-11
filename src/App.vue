<script>
import PageHeader from './components/PageHeader.vue';
import PageMain from './components/PageMain.vue';
import PageFooter from './components/PageFooter.vue';


export default {
  data() {
    return {
      navLinksSx: [
        {
          icon: "/svg-0.svg",
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
      ],
      navLinksDx: [
        {
          icon: "/svg-1.svg",
          href: "#cart",
          text: "CART",
        },
        {
          icon: "fa-solid fa-magnifying-glass",
          href: "#search",
          text: "SEARCH",
        },

      ]

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
    <PageHeader :arrayNavSX="navLinksSx" :arrayNavDX="navLinksDx" />
  </header>
</template>

<style lang="scss">
@use "./styles/general.scss";
@use "./styles/partials/variables" as *;

header {
  height: 500px;
  background-color: $background-color-first;
  // background-color: #8F8F8F;
  padding-top: 70px;

  background-size: 100px 100px;
  /* dimensione dei punti */
  background-image: radial-gradient(#8F8F8F 1px, transparent 0);
  /* effetto puntinato */

}
</style>
