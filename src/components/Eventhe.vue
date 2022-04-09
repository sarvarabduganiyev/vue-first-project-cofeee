<script>
import Sarlavha from './Sarlavha.vue';
export default {
  components: { Sarlavha },};
</script>

<template>
  <div class="big__content">
    <h1>
      Even the all-powerful Pointing has no control about the blind texts.
    </h1>
    <h2>
      It is a paradisematic country, in which roasted parts of sentences fly
      into your mouth. Even the all-powerful Pointing has no control about the
      blind texts it is an almost unorthographic life One day however a small
      line of blind text by the name of Lorem Ipsum decided to leave for the far
      World of Grammar.
    </h2>
    <div class="read__theDiv flex flex-col justify-center items-center">
      <button>Read the full Story</button>
      <div class="line__btn"></div>
    </div>
    <Sarlavha word="Featured Mugs" />
   </div>
</template>


<style scoped>
h1 {
  font-style: normal;
  font-weight: 400;
  font-size: 28px;
  line-height: 40px;
  text-align: center;
  color: #1d1f2e;
}
h2 {
  margin-top: 16px;
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 28px;
  text-align: center;
  color: rgba(29, 31, 46, 0.7);
}

button {
  font-style: normal;
  font-weight: 400;
  font-size: 15px;
  line-height: 28px;
  text-align: center;
  color: #a25f4b;
}
.line__btn {
  background: rgba(162, 95, 75, 0.2);
  height: 2px;
  display: inline-block;
  width: 133px;
}

.big__content {
  margin-top: 120px;
  padding: 0px 350px;
}
.read__theDiv {
  margin-top: 20px;
}

@media (max-width: 1297px) {
  .big__content {
    margin-top: 100px;
    padding: 0px 200px;
  }
}
@media (max-width: 1177px) {
  .big__content {
    margin-top: 70px;
    padding: 0px 100px;
  }
}
@media (max-width: 762px) {
  .big__content {
    margin-top: 40px;
    padding: 0px 50px;
  }
  h1 {
    font-size: 20px;
    line-height: 30px;
  }
  h2 {
    margin-top: 12px;
    font-size: 12px;
    line-height: 22px;
  }

  button {
    font-size: 12px;
    line-height: 30px;
  }
 
}
@media(max-width:506px){
   .big__content {
    margin-top: 30px;
    padding: 0px 20px;
  }
}
@media(max-width:360px){
   .big__content {
    margin-top: 50px;
    padding: 0px 10px;
  }
}
</style>