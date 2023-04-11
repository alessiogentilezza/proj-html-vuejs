<script>
import PageHeader from './components/PageHeader.vue';
import PageMain from './components/PageMain.vue';
import PageFooter from './components/PageFooter.vue';


export default {
  data() {
    return {
      
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

  <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Consectetur ea totam omnis quis, aut, consequuntur architecto autem cumque possimus error minus expedita in debitis! Veniam amet ducimus illum modi iure, eaque nisi totam recusandae consequatur! Consectetur, doloremque quisquam harum cumque et reiciendis tempora iste, sed consequuntur magni libero eos illum.</p>

</template>

<style lang="scss">
@use "./styles/general.scss";
@use "./styles/partials/variables" as *;

p{
  color: $rosso;
}
</style>
