<template>
  <nav class="my-container">

    <!-- LINK NAVBAR SX -->
    
    <div class="col-25">
      <button t class="my-btn">ORDER ONLINE</button>
    </div>
    
    <!-- LINK NAVBAR CC -->
    
    <div class="col-50">
      <ul class="navbar-links cc">
        <li v-for="(link, i) in arrayNavSX" :key="i">
          <img v-if="link.icon != ''" class="img-small" :src="link.icon" alt="">
          <img id="logo" :src="link.logo" alt="">
          <a v-if="link.text != ''" class="nav-link" :href="link.href">{{ link.text }}</a>
        </li>
      </ul>
    </div>
    
    <!-- LINK NAVBAR DX -->
    
    <div class="col-25">
      <ul class="navbar-links dx">
        <li v-for="(link, i) in arrayNavDX" :key="i">
          <img v-if="link.icon != ''" class="img-small" :src="link.icon" alt="">
          <i :class="link.icon"></i>
          <a class="nav-link" :href="link.href">{{ link.text }}</a>
        </li>
      </ul>
    </div>
  </nav>
  <div class="wrap">
    <img src="/h3-rev-img-5.png" alt="">
    <img id="pizza-top" src="/h3-rev-img-6.png" alt="">
  </div>
</template>

<script>
export default {
  name: 'PageHeader',
  props: {
    arrayNavSX: Array,
    arrayNavDX: Array,
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
nav.my-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 50px;
}
.navbar-links {
  display: flex;
}
ul.navbar-links.cc {
  justify-content: center;
}
ul.navbar-links.dx {
  justify-content: flex-end;
}
.my-btn {
  background-color:$background-color-second;
  color:$text-color-white;
  padding: 1rem;
  border: none;
  cursor: pointer;
}
.nav-link {
  padding: 0 1rem;
  text-decoration: none;
  color:$text-color-white;
}
.col-25{
  width: 25%;
}
.col-50 {
  width: 50%;
}
li {
  height: 100%;
  display: flex;
  align-items: center;
  color:$text-color-white;
}
.img-small {
  filter: invert(1);
  height: 10px;
}
#logo {
  height: 70px;
  text-align: center;
}
.wrap {
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 90%;
  & img {
    height: 80%;
  }
}
#pizza-top {
  position: absolute;
  z-index: 10;
}</style>