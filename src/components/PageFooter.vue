<template>
  <div id="footer" class="d-flex">

<!-- COLONNA SX 1 -->

    <div class="col sx-txt logo-wrap">
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
      <div class="d-flex sign items-center">
        <p class="text-color-gold">Create with &hearts; by</p>&nbsp&nbsp<p class="text-color-green">Qode
          Interactive</p>
      </div>
    </div>

<!-- COLONNA SX 2 -->

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
            <span>
              <i :class="link.icon1"></i>
              <i :class="link.icon2"></i>
              <i :class="link.icon3"></i>
              <i :class="link.icon4"></i>
            </span>
          </li>
        </ul>
      </div>
    </div>

<!-- COLONNA SX 3 -->

    <div class="col sx-txt logo-wrap">
      <h4 class="text-color-white ">
        THE DON PEPPE CREW FIRST AND FOREMOST
        VALUES AN AUTHENTIC, WELL BAKED SLICE OF PIZZA.
      </h4>
      <img src="/h5-logo-divided-header.png" alt="">
    </div>

<!-- COLONNA DX IMG -->

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
}

.col.sx-txt {
  padding-top: 5rem;
  padding-left: 2rem;

  span {
    font-size: 16px;

    i {
      padding-right: .4rem;
      color: $text-color-white;
      font-size: 10px;
    }
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

.img {
  width: 20px;
}

.logo-wrap {
  position: relative;

  img {
    position: absolute;
    bottom: 50px;
    left: 50px;
    height: 100px;
  }
}

.sign {
  position: absolute;
  bottom: 20px;
  left: 20px;
  font-size: 10px;
  line-height: 12px;

}
</style>