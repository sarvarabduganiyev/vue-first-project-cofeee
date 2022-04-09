<script>
export default {};
</script>
<template>
  <section>
    <div class="glavniy__div">
      <h3>Sign up and get free coffee bags</h3>
      <h1>Coffee Updates</h1>
      <div class="btnBox flex justify-center items-center">
        <button class="customer">customer @coffestyle.io</button>
        <button class="subscribe">subscribe</button>
      </div>
    </div>
  </section>
</template>

<style scoped>
h1 {
  margin-top: 15px;
  font-style: normal;
  font-weight: 400;
  font-size: 36px;
  line-height: 50px;
  text-align: center;
  color: #ffffff;
}
h3 {
  font-style: normal;
  font-weight: 400;
  font-size: 12px;
  line-height: 18px;
  text-align: center;
  letter-spacing: 2px;
  text-transform: uppercase;
  color: #ffffff;
}
.customer {
  font-style: normal;
  font-weight: 400;
  font-size: 12px;
  line-height: 18px;
  text-align: center;
  letter-spacing: 2px;
  text-transform: uppercase;
  color: #ffffff;
  padding: 18px 40px;
  border: 1px solid #2f303e;
}
.subscribe {
  font-weight: 400;
  font-size: 12px;
  line-height: 18px;
  text-align: center;
  letter-spacing: 2px;
  text-transform: uppercase;
  color: #000000;
  padding: 18px 25px;
  background-color: white;
  margin-left: 10px;
}
.glavniy__div {
  background-color: #1d1f2e;
  padding: 80px 400px;
}
.btnBox {
  margin-top: 15px;
}
@media (max-width: 1250px) {
  .glavniy__div {
    padding: 80px 200px;
  }
}
@media (max-width: 830px) {
  .glavniy__div {
    padding: 80px 20px;
  }
}
@media (max-width: 830px) {
  .glavniy__div {
    padding: 80px 20px;
  }
  h1 {
    margin-top: 10px;
    font-size: 30px;
    line-height: 40px;
  }
  h3 {
    font-size: 10px;
    line-height: 15px;
    letter-spacing: 1px;
  }
  .customer {
    font-size: 10px;
    line-height: 15px;
    letter-spacing: 1px;
    padding: 10px 40px;
    margin-top: 10px;
  }
  .subscribe {
    font-size: 10px;
    line-height: 15px;
    letter-spacing: 1px;
    padding: 10px 20px;
    margin-left: 10px;
  }
}
@media (max-width: 400px) {
  .glavniy__div {
    padding: 50px 10px;
  }
  .btnBox {
    flex-direction: column-reverse;
  }
}
</style>