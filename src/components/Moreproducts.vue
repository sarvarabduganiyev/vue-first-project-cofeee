<script>
import Allcofee from "./Allcofee.vue";
import Sarlavha from "./Sarlavha.vue";
export default {
  data() {
    return {
      datas: [
        {
          sarlavha: "Red Love Cup",
          font: "$25.00",
          span: "$ 37.00 USD",
          imageUrl: "/src/img/card/1.png",
        },
        {
          sarlavha: "Black Tea Cup",
          font: "$15.00",
          span: "$ 29.00 USD",
          imageUrl: "/src/img/card/2.png",
        },
        {
          sarlavha: "B&W Essentials Mug",
          font: "$ 19.00 USD",
          span: "",
          imageUrl: "/src/img/card/3.png",
        },
        {
          sarlavha: "Winter Style Mug",
          font: "$25.00",
          span: "",
          imageUrl: "/src/img/card/4.png",
        },
        {
          sarlavha: "Ceramic Tea",
          font: "$46.00",
          span: "",
          imageUrl: "/src/img/card/5.png",
        },
        {
          sarlavha: "No Handle Bar Cup",
          font: "$34.00",
          span: "",
          imageUrl: "/src/img/card/6.png",
        },
        {
          sarlavha: "Espresso Cup by Mugs.co",
          font: "$25.00",
          span: "",
          imageUrl: "/src/img/card/7.png",
        },
        {
          sarlavha: "Pink Premium Ceramic",
          font: "$99.00",
          span: "",
          imageUrl: "/src/img/card/8.png",
        },
        {
          sarlavha: "Summer Designer Cup",
          font: "$29.00",
          span: "",
          imageUrl: "/src/img/card/9.png",
        },
      ],
    };
  },
  components: { Sarlavha, Allcofee },
};
</script>

<template>
  <div>
    <Sarlavha word="More Products" />
    <div class="flex justify-center flex-col items-center">
      <div class="gridDiv">
        <div v-for="malumot in datas" :key="malumot.sarlavha">
          <Allcofee :malumot="malumot" />
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.gridDiv {
  padding: 100px 250px;
  width: 100%;
  display: grid;
  grid-template-columns: calc(33.3% - 6px) calc(33.3% - 6px) calc(33.3% - 6px);
  gap: 18px;
}
@media (max-width: 1243px) {
  .gridDiv {
    padding: 100px 150px;
  }
}
@media (max-width: 1050px) {
  .gridDiv {
    padding: 100px 50px;
  }
}
@media (max-width: 850px) {
  .gridDiv {
    padding: 100px 50px;
    grid-template-columns: calc(50% - 10px) calc(50% - 10px);
    gap: 20px;
  }
}

@media (max-width: 615px) {
  .gridDiv {
    width: 100%;
    padding: 100px 50px;
    grid-template-columns: repeat(1, 1fr);
    gap: 20px;
  }
}
@media (max-width: 500px) {
  .gridDiv {
    /* width: 100%; */
    padding: 100px 20px;
    grid-template-columns: repeat(1, 1fr);
    gap: 20px;
  }
}
</style>