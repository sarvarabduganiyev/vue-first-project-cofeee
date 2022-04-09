<script>
export default {};
</script>

<template>
  <section>
    <div class="megaDiv">
      <div class="coffee__Bg">
        <div>
          <h3 class="best">Best place to buy design</h3>
          <h1 class="coffeeMugs">Coffee Mugs</h1>
          <h3 class="the__most">
            The most versatile furniture system ever created. Designed to fit
            your life, made to move and grow.
          </h3>
          <div class="flex flex-col justify-center items-center">
            <button>Explore Our Products</button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>


<style scoped>
.megaDiv {
  padding: 0px 20px;
}
.coffee__Bg {
  background-image: url("../img/bg.png");
  background-position: bottom;
  background-size: cover;
  height: 540px;
}
.best {
  padding-top: 152px;
  font-style: normal;
  font-weight: 400;
  font-size: 12px;
  line-height: 18px;
  text-align: center;
  letter-spacing: 2px;
  text-transform: uppercase;
  color: #ffffff;
}
.coffeeMugs {
  font-style: normal;
  font-weight: 400;
  font-size: 47px;
  line-height: 60px;
  text-align: center;
  color: #ffffff;
  margin-top: 10px;
}
.the__most {
  margin-top: 10px;
  font-style: normal;
  font-weight: 400;
  font-size: 17px;
  line-height: 30px;
  text-align: center;
  color: #ffffff;
}
button {
  margin-top: 48px;
  font-style: normal;
  font-weight: 400;
  font-size: 12px;
  line-height: 18px;
  text-align: center;
  letter-spacing: 2px;
  text-transform: uppercase;
  color: #1d1f2e;
  padding: 0px 24px;
  background-color: #fff;
}
@media (max-width: 921px) {
  .megaDiv {
    padding: 0px;
  }
  .coffee__Bg {
    padding: 0px 30px;
  }
}
@media (max-width: 520px) {
  /* .coffee__Bg {
  background-image: url("../img/bg.png");
  background-position: bottom;
  background-size: cover;
  height: 540px;
} */
  .best {
    padding-top: 152px;
    font-size: 10px;
    line-height: 15px;
    text-align: center;
    letter-spacing: 1px;
  }
  .coffeeMugs {
    font-size: 32px;
    line-height: 45px;
    margin-top: 7px;
  }
  .the__most {
    margin-top: 7px;
    font-size: 15px;
    line-height: 28px;
  }
  button {
    margin-top: 30px;
    font-size: 10px;
    line-height: 15px;
    letter-spacing: 1px;
    padding: 0px 10px;
  }
}
</style>