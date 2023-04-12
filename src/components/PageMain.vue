<template>
  <!-- PRIMA SEZIONE -->

  <section class="no-margin col-4 first">
    <ul class="d-flex">
      <li><img src="/h3-img-1.jpg" alt=""></li>
      <li><img src="/h3-img-2.jpg" alt=""></li>
      <li><img src="/h3-img-3.jpg" alt=""></li>
      <li><img src="/h3-img-4.jpg" alt=""></li>
    </ul>
  </section>

  <!-- SEDONDA SEZIONE -->

  <section class="no-margin">
    <div class="title txt-dark-gray">
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

  <!-- TERZA SEZIONE -->

  <section>
    <div class="d-flex">
      <div class="col sx-img">
        <img id="img-back" src="/h1-img-4.jpg" alt="">
        <img id="img-front" src="/h1-img-7n.png" alt="">
      </div>
      <div class="col dx-txt">
        <h3>SPECIALS*</h3>
        <div class="txt-light-gray">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam, iusto?</div>
        <h5 class="price">$10</h5>
        <h5>COMBO PICCOLO</h5>
        <p class="txt-light-gray">Lorem ipsum dolor sit amet.</p>
        <h5 class="price">$20</h5>
        <h5>COMBO MEZZO</h5>
        <p class="txt-light-gray">Lorem ipsum dolor sit amet.</p>
        <h5 class="price">$30</h5>
        <h5>COMBO GRANDE</h5>
        <p class="txt-light-gray">Lorem ipsum dolor sit amet.</p>
      </div>
    </div>
  </section>

  <!-- QUARTA SEZIONE -->

  <section>
    <div class="d-flex wrap">
      <div class="small sx top"></div>
      <div class="small center top"></div>
      <div class="small dx top"></div>

      <div class="big sx"></div>
      <div class="big center">
        <p class="text-color-white">GO AHEAD AND BUILD YOUR OWN PIZZA WE WON'T JUDGE!</p>
      </div>

      <div class="big dx"></div>

      <div class="small sx bottom"></div>
      <div class="small center bottom"></div>
      <div class="small dx bottom"></div>
    </div>



  </section>

  <!-- QUINTA SEZIONE -->

  <section class="col-4">
    <ul class="d-flex">
      <li><img src="/h1-team-1a-700x700.jpg"></li>
      <li><img src="/h1-team-2a.jpg"></li>
      <li><img src="/h1-team-3a.jpg"></li>
      <li><img src="/h1-team-4a.jpg"></li>
    </ul>
  </section>

  <!-- SESTA SEZIONE -->

  <section id="clients-sec" class="col-5 ">
    <ul class="d-flex">
      <li><img src="/h1-clients-img-1.png"></li>
      <li><img src="/h1-clients-img-2.png"></li>
      <li><img src="/h1-clients-img-3.png"></li>
      <li><img src="/h1-clients-img-4.png"></li>
      <li><img src="/h1-clients-img-5.png"></li>
    </ul>
  </section>

  <!-- SETTIMA SEZIONE -->

  <section class="col-6">
    <ul class="d-flex space-between" >
      <li class="pizza-wrap"><img class="pizza left" src="/h3-product-img-1a-100x100.png"></li>
      <li><img src="/h3-product-img-2a-150x150.png"></li>
      <li><img src="/h3-product-img-3a-150x150.png"></li>
      <li><img src="/h3-product-img-4a-150x150.png"></li>
      <li><img src="/h3-product-img-5a-150x150.png"></li>
      <li class="pizza-wrap"><img class="pizza right" src="/h3-product-img-6a-100x100.png"></li>
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

ul {
  margin: 5px 0;
  justify-content: center;


  li img {
    width: 100%;
  }
}

.col-4 li {
  width: calc(100% / 4);
}

.col-4.first li {
  margin: 0 2.5px;
}

#clients-sec{
  background-color: $background-color-third;
}
.col-5 li {
  width: calc(100% / 10);
}

.pizza-wrap {
  position: relative;
}
.pizza{
  position: absolute;
    top: -75px;
    z-index: 10;
    width: 150px;


}
.pizza.left{
    left: -75px;
}
.pizza.right{
    right: -75px;
}

p i {
  color: $text-color-gold;
  font-size: 70px;
}

h6 {
  color: $text-color-red;
  padding: .1rem;
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

#img-back {
  width: 100%;
}

.col {
  position: relative;
  width: 50%;

  p {
    padding-left: 40px;
  }
}

#img-front,
.title {
  width: 50%;
  text-align: center;
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
}

.col.dx-txt {
  padding: 0 5rem;
}

h5 {
  display: inline-block;
  padding: 1rem 1rem 1rem 0;
}

h3 {
  padding: 1rem 0;
}

.price {
  color: $text-color-red;
}

.text-color-white {
  color: $text-color-white;
}

.txt-dark-gray {
  color: $text-color-dark-gray;
}

.txt-light-gray {
  color: $text-color-light-gray;
}

.small {
  height: 100px;
}

.big {
  height: 200px;

}

.center {
  width: 90%;
}

.sx,
.dx {
  width: 5%;
}

.small.sx.top {
  background-image: url(/h3-background-img.jpg);
  background-repeat: no-repeat;
  background-position-y: 100%;
  background-position-x: 100%;
}

.small.sx.bottom {
  background-image: url(/h3-background-img.jpg);
  background-repeat: no-repeat;
  background-position-y: 70%;
  background-position-x: 100%;
}

.small.center.top {
  background-image: url(/h3-background-img.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  background-position-y: 100%;
  // background-position-x: 100%;
}

.small.center.bottom {
  background-image: url(/h3-background-img.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  background-position-y: 70%;
  background-position-x: 100%;
}

.small.dx.top {
  background-image: url(/h3-background-img.jpg);
  background-repeat: no-repeat;
  background-position-y: 0%;
  background-position-x: 0%;
}

.small.dx.bottom {
  background-image: url(/h3-background-img.jpg);
  background-repeat: no-repeat;
  background-position-y: 70%;
  background-position-x: 0%;
}

.big.sx {
  background-image: url(/h3-background-img.jpg);
  background-repeat: no-repeat;
  background-position-y: 0%;
  background-position-x: 100%;
}

.big.center {
  position: relative;
  background-image: url(/h3-background-img.jpg);
  background-size: 200%;
  background-repeat: no-repeat;
  background-size: 140%;
  background-position-x: 70%;
  background-position-y: 15%;

  p {
    position: absolute;
    z-index: 10;
    left: 10%;
    top: -10%;
    width: 30%;
    font-size: 40px;
    font-weight: bolder;
  }
}


.big.dx {
  background-image: url(/h3-background-img.jpg);
  background-repeat: no-repeat;
  background-position-y: 50%;
  background-position-x: 0%;
}
</style>

