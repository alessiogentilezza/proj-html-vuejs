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
          icon: "",
          href: "#pages",
          text: "PAGES",
        },
        {
          icon: "",
          href: "#menu",
          text: "MENU",
        },
        {
          icon: "",
          logo: "/h5-logo-divided-header.png",
          text: "",

        },

        {
          icon: "",
          href: "#event",
          text: "EVENT",
        },
        {
          icon: "",
          href: "#blog",
          text: "BLOG",
        },
        {
          icon: "",
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
  // display: flex;
  // flex-direction: column;
  background-color: $background-color-first;
  padding-top: 30px;

  // background-color: #8F8F8F;

    background-size: 100px 100px;
  background-image: radial-gradient(#8F8F8F 1px, transparent 0);
  

}
</style>
