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
      ],
      arrayFooterFirst: [
        {
          title: "FIND OUR RESTAURANTS",
          links1: [
            "1614 E. Bell Rd #104",
            "Salerno, AZ 85022",
            "(602) 867-1010",
          ]
        },
        {
          links2: [
            "204 E. Pizzetta Tommaso",
            "Sorrento, AZ 85022",
            "(358) 867-1010",
          ]
        },
        {
          links3: [
            "Via Puglia 54",
            "Torre Del Greco AZ 85022",
            "(359) 867-1010",
          ]
        },
        {
          links4: [
            "Corso Italia",
            "Naples, AZ 85022",
            "989) 867-1010",
          ]
        },
      ],
      arrayFooterSecond: [
        {
          title: "WORKING HOURS",
          day: "MONDAY",
          timeClose: "Kitchen Closed",
        },
        {
          day: "TUSEDAY UNTIL FRIDAY",
          time: "9:00 - 22:00",
        },
        {
          day: "SATURDAY",
          time: "Saturday 11am to midnight",
        },
        {
          day: "SUNDAY",
          time: "9:00 - 22:00",
        },
        {
          day: "FOLLOW US",
          icon1: "fa-brands fa-twitter",
          icon2: "fa-brands fa-facebook",
          icon3: "fa-brands fa-instagram",
          icon4: "fa-brands fa-linkedin",
          day2: "FOLLOW US",
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
  <main>
    <PageMain />
  </main>
  <footer>
    <PageFooter :arrayFooterFirst="arrayFooterFirst" :arrayFooterSecond="arrayFooterSecond" />
  </footer>
</template>

<style lang="scss">
@use "./styles/general.scss";
@use "./styles/partials/variables" as *;

header {
  height: 500px;
  background-color: $background-color-first;
  padding-top: 30px;
  background-size: 100px 100px;
  background-image: radial-gradient(#8F8F8F 1px, transparent 0);
}
</style>
