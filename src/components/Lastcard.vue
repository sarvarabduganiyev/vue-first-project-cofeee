<script>
export default {
    props:{
        data:{
            required:true,
            type:Object
        }
    }
};
</script>
<template>
  <div>
    <div class="relative lastCard__imgBox">
      <img
        class="w-full h-full absolute object-cover"
        :src="data.imageURL"
        alt="11"
      />
    </div>
    <div>
      <h1>
       {{data.hash1}}
      </h1>
      <h2>
        {{data.hash2}}
      </h2>
      <h3>{{data.hash3}}</h3>
    </div>
  </div>
</template>

<style scoped>
h1 {
  font-style: normal;
  font-weight: 400;
  margin-top: 29px;
  font-size: 20px;
  line-height: 32px;
  color: #1d1f2e;
}
h2 {
  margin-top: 10px;
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 28px;
  color: rgba(29, 31, 46, 0.7);
}
h3 {
  margin-top: 16px;
  font-style: normal;
  font-weight: 400;
  font-size: 12px;
  line-height: 18px;
  letter-spacing: 2px;
  text-transform: uppercase;
  color: #1d1f2e;
}
.lastCard__imgBox {
  height: 300px;
}
</style>