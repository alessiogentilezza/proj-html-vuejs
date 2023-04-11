<template>
  <section class="no-margin first">
<ul class="d-flex">
  <li><img src="/h3-img-1.jpg" alt=""></li>
  <li><img src="/h3-img-2.jpg" alt=""></li>
  <li><img src="/h3-img-3.jpg" alt=""></li>
  <li><img src="/h3-img-4.jpg" alt=""></li>
</ul>    
  </section>

  <section class="no-margin">
    <div class="title">
          <h3>"FORGET THE TRENDY PI77A SHOPS THIS HINDEN SPOT MAKES THE BEST NEW YORK-STYLE PIZZA SLICE IN NAPLES"</h3>

    </div>

<ul class="d-flex">
  <li><img src="/h3-testimonials-bckgrnd.jpg" alt=""></li>
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
  .first li{
    width: calc(100% / 4);
    list-style: none;
    margin: 0 5px;
  }

  img {
    width:  100%;
  }

  .title{
    width: 50%;
    text-align: center;
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);


  }

</style>