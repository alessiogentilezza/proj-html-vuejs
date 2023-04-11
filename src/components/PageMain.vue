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
      <p><i class="fa-solid fa-quote-left"></i></p>
      <h3>"FORGET THE TRENDY PI77A SHOPS THIS HINDEN SPOT MAKES THE BEST NEW YORK-STYLE PIZZA SLICE IN NAPLES"</h3>
      <h6>WASHINGTON POST 2018</h6>
      <ul class="d-flex">
        <li class="circle first"></li>
        <li class="circle"></li>
        <li class="circle"></li>
      </ul>
    </div>
    <ul class="d-flex">
      <li><img src="/h3-testimonials-bckgrnd.jpg" alt=""></li>
    </ul>
  </section>

  <section>
    <div class="d-flex">
      <div class="col">
        <img src="/h1-img-4.jpg" alt="">

      </div>
      <div class="col dx">
        <h3>SPECIALS*</h3>
        <div class="txt">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam, iusto?</div>        
        <h5 class="price">$10</h5><h5>COMBO PICCOLO</h5>
        <p class="txt">Lorem ipsum dolor sit amet.</p>
        <h3>SPECIALS*</h3>
        <p class="txt">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam, iusto?</p>
        <h5 class="price">$20</h5><h5>COMBO PICCOLO</h5>
        <p class="txt">Lorem ipsum dolor sit amet.</p>
        <h3>SPECIALS*</h3>
        <p class="txt">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam, iusto?</p>
        <h5 class="price">$30</h5><h5>COMBO PICCOLO</h5>
        <p class="txt">Lorem ipsum dolor sit amet.</p>
      </div>
    </div>

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

ul {
  margin: 5px 0;

}

.first li {
  width: calc(100% / 4);
  list-style: none;
  margin: 0 2.5px;
}

img {
  width: 100%;
}

.title {
  width: 50%;
  text-align: center;
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  color: $text-color-gray;
}

p i {
  color: $text-color-gold;
  font-size: 70px;
}

h6 {
  color: $text-color-red;
  padding: 1rem;

}

.circle {
  height: 10px;
  width: 10px;
  border-radius: 50%;
  background-color: #EBEBDE;
  margin: 1rem 0.2rem;
  list-style: none;

}

.circle.first {
  background-color: #B7903C;
}
.col {
  width: 50%;
  p{
    padding-left: 2rem;
  }
}
.col.dx{
padding: 5rem;}

h5{
  display: inline-block;
  padding: 1rem 1rem 1rem 0;
}
h3{
  padding:1rem 0;
}
.price{
  color: $text-color-red;

}
.txt{
  color: #888888;

}
</style>