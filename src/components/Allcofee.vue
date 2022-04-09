<script>
export default {
  props: {
    malumot: {
      type: Object,
      required: true,
    },
  },
};
</script>
<template>
  <div>
    <div class="relative" style="height: 380px">
      <img
        class="absolute w-full h-full object-cover"
        :src="malumot.imageUrl"
        alt="card1"
      />
    </div>
    <div>
      <h2 class="text-center">{{ malumot.sarlavha }}</h2>
      <h3 class="text-center"><font>{{ malumot.font }} </font> <span> {{ malumot.span }}</span></h3>
    </div>
  </div>
</template>
<style scoped>
h2 {
  font-style: normal;
  font-weight: 400;
  font-size: 20px;
  line-height: 30px;
  text-align: center;
  color: #1d1f2e;
  margin-top: 35px;
}
h3 font {
  margin-top: 8px;
  font-style: normal;
  font-weight: 400;
  font-size: 19px;
  line-height: 32px;
  text-align: center;
  color: #a25f4b;
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
</style>