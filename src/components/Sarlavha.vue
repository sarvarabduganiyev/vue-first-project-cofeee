<script>
export default {
  props: {
    word: {
      type: String,
      required: true,
    },
  },
};
</script>
<template>
  <div class="featured__div flex justify-center items-center">
    <div class="h3__line"></div>
    <h3 class="featured mx-3">{{ word }}</h3>
    <div class="h3__line"></div>
  </div>
</template>


<style scoped>
.featured__div {
  margin-top: 100px;
}
.h3__line {
  background: #ececed;
  display: inline-block;
  width: 30px;
  height: 1px;
}
h3 {
  font-style: normal;
  font-weight: 400;
  font-size: 12px;
  line-height: 18px;
  text-align: center;
  letter-spacing: 2px;
  text-transform: uppercase;
  margin: 0px 15px;
}
@media (max-width: 762px) {
  h3 {
    font-size: 10px;
    line-height: 15px;
    letter-spacing: 1px;
    margin: 0px 12px;
  }
  .featured__div {
    margin-top: 50px;
  }
}
</style>