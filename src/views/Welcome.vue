<template>
  <div class="home">
    <img alt="background" src="../assets/BG.png" class="background" />
    <img alt="img cripto" src="../assets/IMG.png" class="img-welcome" />
    <div class="title">
      <h1>hola</h1>
      <h3>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Et nam culpa
        voluptatem vero tenetur quibusdam sint, laboriosam aspernatur vitae,
        odio repellendus accusantium fuga ea repellat magni corrupti consectetur
        nihil labore!
      </h3>
      <vs-button
        transparent
        :active="btnActive == 1"
        @click="btnActive = 1"
        class="container-btn"
      >
        <img :src="getStarted" alt="" class="btn-get-started" />
      </vs-button>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
/* import HelloWorld from '@/components/HelloWorld.vue' */
import getStarted from "@/assets/getStarted.png";

export default {
  name: "Home",

  data: () => ({
    btnActive: 0,
    getStarted: getStarted,
  }),
  components: {
    /* HelloWorld */
  },
};
</script>

<style scoped>
.background {
  position: absolute;
  width: 1613px;
  height: 816.31px;
  left: -35px;
}
.img-welcome {
  position: absolute;
  width: 628px;
  height: 519px;
  left: 828px;
}
.title {
  position: absolute;
}
.btn-get-started {
  width: 157px;
  height: 54px;
  border-radius: 100px;
}
</style>
