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
<div>
<ul>
  <li><img src="src/assets/svg/svg-0.svg" alt=""></li>
  <li><img src="src/assets/svg/svg-1.svg" alt=""></li>
  <li><img src="src/assets/svg/svg-2.svg" alt=""></li>
  <li><img src="src/assets/svg/svg-3.svg" alt=""></li>
  <li><img src="src/assets/svg/svg-4.svg" alt=""></li>
  <li><img src="src/assets/svg/svg-5.svg" alt=""></li>
  <li><img src="src/assets/svg/svg-6.svg" alt=""></li>
  <li><img src="src/assets/svg/svg-7.svg" alt=""></li>
  <li><img src="src/assets/svg/svg-8.svg" alt=""></li>
  <li><img src="src/assets/svg/svg-9.svg" alt=""></li>
  <li><img src="src/assets/svg/svg-10.svg" alt=""></li>
  <li><img src="src/assets/svg/svg-11.svg" alt=""></li>
</ul>


</div>
</template>

<style lang="scss">
@use "./styles/general.scss";
@use "./styles/partials/variables" as *;

p{
  color: $rosso;
}
img{
  background-color: rebeccapurple;
  height: 100px;
}
</style>
