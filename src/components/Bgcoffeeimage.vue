<script>
import Lastcard from "./Lastcard.vue";
import Sarlavha from "./Sarlavha.vue";
export default {
  components: { Sarlavha, Lastcard },
  data(){
      return{
          cardData:[
              {
                  hash1:"Health Check: why do I get a headache when I haven’t had my coffee?",
                  hash2:"It is a paradisematic country, in which roasted parts of sentences fly into your mouth.",
                  hash3:"October 9, 2018",
                  imageURL:"/src/img/card/11.png"
              },
              {
                  hash1:"How long does a cup of coffee keep you awake?",
                  hash2:"It is a paradisematic country, in which roasted parts. Vel qui et ad voluptatem.",
                  hash3:"October 9, 2018",
                  imageURL:"/src/img/card/22.png"
              },
              {
                  hash1:"Recent research suggests that heavy coffee drinkers may reap health benefits.",
                  hash2:"It is a paradisematic country, in which roasted parts of sentences fly into your mouth.",
                  hash3:"October 9, 2018",
                  imageURL:"/src/img/card/33.png"
              },
          ]
      }
  }
};
</script>
<template>
  <section>
    <div class="relative coffeeBG">
      <img
        src="../img/coffeeBG.png"
        class="absolute w-full h-full object-cover"
        alt="coffeeBG"
      />
    </div>
    <div>
      <Sarlavha word="Behind the mugs, lifestyle stories" />
    </div>
    <div class="gridDiv">
      <div v-for="data in cardData" :key="data.hash1">
          <Lastcard :data="data" />
      </div>
    </div>
  </section>
</template>

<style scoped>
.coffeeBG {
  height: 340px;
}
.gridDiv{
    display: grid;
    grid-auto-columns:calc(33.3 - 7px) calc(33.3 - 7px) calc(33.3 - 7px) ;
    gap: 21px;
}
</style>