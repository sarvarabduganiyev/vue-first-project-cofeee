<script>
import Sarlavha from "./Sarlavha.vue";
export default {
  components: { Sarlavha },
};
</script>

<template>
  <Sarlavha word="Buy 2 mugs and get a coffee magazine free" />
  <div class="big__Div">
    <div>
      <div class="parent">
        <div style="height: 280px; width: 260px" class="div6 relative">
          <img
            class="absolute w-full h-full object-cover"
            src="../img/grid3.png"
            alt="grid3"
          />
        </div>
        <div
          style="height: 130px; width: 160px"
          class="div1 relative bg-red-400"
        >
          <img
            class="absolute w-full h-full object-cover"
            src="../img/grid1.png"
            alt="grid1"
          />
        </div>
        <div style="height: 130px; width: 160px" class="div2 relative">
          <img
            class="absolute w-full h-full object-cover"
            src="../img/grid2.png"
            alt="grid2"
          />
        </div>
      </div>
    </div>
    <div class="shopping__Div">
      <h2>Premium Offer</h2>
      <h1>Get our Coffee Magazine</h1>
      <h3>
        The most versatile furniture system ever created. Designed to fit your
        life.
      </h3>
      <button>Start Shopping</button>
    </div>
  </div>
</template>

<style scoped>
.parent {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: repeat(2, 1fr);
  grid-column-gap: 20px;
  grid-row-gap: 20px;
}

.div1 {
  grid-area: 1 / 1 / 2 / 2;
}
.div2 {
  grid-area: 2 / 1 / 3 / 2;
}
.div6 {
  grid-area: 1 / 2 / 3 / 3;
}
.big__Div {
  /* align-items: start; */
  padding: 100px 250px;
  display: grid;
  grid-template-columns: calc(50% - 40px) calc(50% - 40px);
  gap: 80px;
}
.shopping__Div {
  margin-left: 50px;
}
.shopping__Div h2 {
  font-style: normal;
  font-weight: 400;
  font-size: 12px;
  line-height: 18px;
  letter-spacing: 2px;
  text-transform: uppercase;
  color: #1d1f2e;
}
.shopping__Div h1 {
  margin-top: 14px;
  font-style: normal;
  font-weight: 400;
  font-size: 36px;
  line-height: 50px;
  color: #1d1f2e;
}
.shopping__Div h3 {
  margin-top: 16px;
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 28px;
  color: rgba(29, 31, 46, 0.7);
}
.shopping__Div button {
  margin-top: 25px;
  font-style: normal;
  font-weight: 400;
  font-size: 12px;
  line-height: 18px;
  text-align: center;
  letter-spacing: 2px;
  text-transform: uppercase;
  color: #ffffff;
  padding: 9px 24px;
  background-color: #1d1f2e;
  transition: 0.3s ease;
  border: 1px solid #1d1f2e;
}
.shopping__Div button:hover {
  color: #1d1f2e;
  background: #fff;
}
@media (max-width: 1286px) {
  .big__Div {
    /* align-items: start; */
    padding: 100px 200px;
  }
}
@media (max-width: 1194px) {
  .big__Div {
    padding: 100px 150px;
  }
}
@media (max-width: 1094px) {
  .big__Div {
    padding: 100px 100px;
  }
}
@media (max-width: 998px) {
  .big__Div {
    padding: 100px 50px;
  }
}

@media (max-width: 882px) {
  .big__Div {
    padding: 100px 30px;
  }
}
@media (max-width: 814px) {
  .big__Div {
    padding: 100px 30px;
    display: grid;
    grid-template-columns: repeat(1, 1fr);
    gap: 80px;
  }
  .div1 {
    display: none;
    grid-area: initial;
  }
  .div2 {
    display: none;
    grid-area: initial;
  }
  .div6 {
    grid-area: initial;
    width: 100% !important;
  }
  .parent {
    display: grid;
    grid-template-columns: repeat(1, 1fr);
    grid-template-rows: repeat(1, 1fr);
    grid-column-gap: 20px;
    grid-row-gap: 20px;
  }
  .shopping__Div {
    margin-left: 0px;
  }
}
</style>