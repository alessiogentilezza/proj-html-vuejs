<template>
  <nav class="my-container">
    <div>
      <button t class="my-btn">ORDER ONLINE</button>
    </div>
    <div> <!-- LINK NAVBAR -->
      <ul class="navbar-links">
        <li v-for="(link, i) in arrayNavSX" :key="i">
          <img :src=" link.icon " alt="">
          <a class="nav-link" :href="link.href">{{ link.text }}</a>
        </li>
      </ul>
    </div>
    <div>
      <ul class="navbar-links">
        <li v-for="(link, i) in arrayNavDX" :key="i">
          <img :src=" link.icon " alt="">
          <i :class="link.icon"></i>
          <a class="nav-link" :href="link.href">{{ link.text }}</a>
        </li>
      </ul>

    </div>
  </nav>
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

.my-btn {
  background-color: $background-color-second;
  color: $text-color-white;
  padding: 1rem;
  border: none;
  cursor: pointer;
}

.navbar-links {
  display: flex;
  justify-content: center;
  align-items: center;
  list-style: none;
}

.nav-link {
  padding: 0 1rem;
  text-decoration: none;
  display: inline-block;
  color: $text-color-white;
}

nav.my-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 50px;

}
li {
  height: 100%;
  display: flex;
  align-items: center;
  color: $text-color-white;

}
li img{
  filter:invert(1) ;
  height: 16px;
}

</style>