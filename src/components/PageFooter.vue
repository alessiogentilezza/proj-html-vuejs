<template>
  <div id="footer" class="d-flex">

    <div class="col sx-txt">
      <div v-for="(link, i) in arrayFooterFirst" :key="i">
        <h3>{{ link.title }}</h3>
        <ul class="link">
          <li v-for="(data, i) in link.links1" :key="i">
            <h4>{{ data }}</h4>
          </li>
          <li v-for="(data, i) in link.links2" :key="i">
            <h4>{{ data }}</h4>
          </li>
          <li v-for="(data, i) in link.links3" :key="i">
            <h4>{{ data }}</h4>
          </li>
          <li v-for="(data, i) in link.links4" :key="i">
            <h4>{{ data }}</h4>
          </li>
        </ul>
      </div>
    </div>
    <div class="col sx-txt">
      <div v-for="(link, i) in arrayFooterSecond" :key="i">
        <h3>{{ link.title }}</h3>
        <ul class="link">
          <li>
            <div class="d-flex">
              <h4 class="text-color-gold ">{{ link.day }}</h4>
              <span v-if="link.day === 'SATURDAY'" class="text-color-red ">&nbsp*</span>
            </div>
            <h5 class="text-color-red ">{{ link.timeClose }}</h5>
            <h5>{{ link.time }}</h5>
          </li>
        </ul>
      </div>

    </div>
    <div class="col sx-txt"></div>







    <div class="col-dx dx-img">
      <img src="/footer-img-1.jpg" alt="">
    </div>
  </div>
</template>
  
<script>

export default {
  name: 'PageFooter',
  props: {
    arrayFooterFirst: Array,
    arrayFooterSecond: Array
  },


  data() {
    return {
    }
  },

}
</script>
  
<style lang="scss" scoped>
@use "../styles/general.scss";
@use "../styles/partials/variables" as *;

.col {
  width: calc(100% /3);
  border: solid red 1px;
}

.col.sx-txt {
  padding-top: 5rem;
  padding-left: 2rem;
  span{
    font-size: 16px;
  }
}

.col-dx {
  width: 50%;
}

.link {
  padding: 1rem 0;
  list-style: none;
  color: $text-color-light-gray;
  font-size: 12px;
}

h3 {
  color: $text-color-gold;
}
</style>