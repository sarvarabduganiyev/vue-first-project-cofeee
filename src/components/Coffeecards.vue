<script>
export default {
  
};
</script>
<template>
  <section>
    <div class="griDCars">
      <div>
        <div style="height: 540px" class="img__cards__div relative">
          <img
            class="absolute w-full h-full object-cover"
            src="../img/gulli.png"
            alt="gulli"
          />
        </div>
        <div class="golden__word">
          <h2 class="text-center">Pink Premium Ceramic</h2>
          <h3 class="text-center">$ 99.00 USD</h3>
        </div>
      </div>
      <div>
        <div style="height: 540px" class="img__cards__div relative">
          <img
            class="absolute w-full h-full object-cover"
            src="../img/soya.png"
            alt="soya"
          />
        </div>
        <div class="golden__word">
          <h2 class="text-center">Golden Designers Mug</h2>
          <h3 class="text-center">
            <font>$50.00 </font><span> $ 69.00 USD</span>
          </h3>
        </div>
      </div>
    </div>
   
  </section>
</template>


<style scoped>
.griDCars {
  padding: 100px 240px;
  display: grid;
  grid-template-columns: calc(50% - 10px) calc(50% - 10px);
  gap: 20px;
}
h2 {
  font-style: normal;
  font-weight: 400;
  font-size: 20px;
  line-height: 30px;
  text-align: center;
  color: #1d1f2e;
}
h3 {
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 28px;
  text-align: center;
  color: rgba(29, 31, 46, 0.7);
}
h3 span {
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 28px;
  text-align: center;
  text-decoration-line: line-through;
  color: rgba(29, 31, 46, 0.4);
}
h3 font {
  font-style: normal;
  font-weight: 400;
  font-size: 19px;
  line-height: 32px;
  text-align: center;
  color: #a25f4b;
}
@media (max-width: 1258px) {
  .griDCars {
    padding: 100px 100px;
  }
}
@media (max-width: 978px) {
  .griDCars {
    padding: 100px 50px;
  }
}
@media (max-width: 826px) {
  .griDCars {
    padding: 100px 50px;
  }
  .img__cards__div {
    height: 400px !important;
  }
}
@media (max-width: 738px) {
  .griDCars {
    padding: 100px 50px;
    display: grid;
    grid-template-columns: repeat(1,1fr);
    gap: 20px;
  }
  .img__cards__div {
    height: 540px !important;
  }
  .golden__word {
    margin-top: 10px;
  }
}
@media (max-width: 513px) {
  .griDCars {
    padding: 80px 20px;
  }
  .img__cards__div {
    height: 350px !important;
  }
}

</style>