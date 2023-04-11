<template>
  <section class="no-margin">
<ul class="d-flex">
  <li><img src="/h3-img-1.jpg" alt=""></li>
  <li><img src="/h3-img-2.jpg" alt=""></li>
  <li><img src="/h3-img-3.jpg" alt=""></li>
  <li><img src="/h3-img-4.jpg" alt=""></li>
</ul>    
  </section>






  </template>
  
  <script>
  
  export default {
    name: 'PageMain',
  
    data() {
      return {
      }
    },
  
  }
  </script>
  
  <style lang="scss" scoped>
  @use "../styles/general.scss";
  @use "../styles/partials/variables" as *;

ul{
  margin: 10px 0;

}
  li{
    width: calc(100% / 4);
    list-style: none;
    margin: 0 5px;

    & img {
    width:  100%;
  }

  }
</style>