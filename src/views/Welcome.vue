<template>
  <div class="home">
    <img alt="background" src="../assets/BG.png" class="background" />
    <img alt="img cripto" src="../assets/IMG.png" class="img-welcome" />
    <div class="row">
      <div class="col-6 container-left">
        <div class="title">
          We provide easy solution to exchange your
          <b>Bitcoin/ GiftCard for money</b>
        </div>
        <div class="subtitle">
          CoinBase is a platform for trading your bitcoin and giftcard at the
          best rate, why not give us a trial.
        </div>
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

@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@1,200&display=swap');

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
.container-left {
  position: absolute;
  text-align: left;
  padding: 142px;
  padding-right: 0;
}
.title {
  height: 180px;
  display: contents;

  font-family: Poppins;
  font-style: normal;
  font-weight: normal;
  font-size: 40px;
  line-height: 60px;

  color: #ffffff;
  padding-bottom: 30px;
}
.subtitle {
  width: 460px;
  height: 54px;

  font-family: Poppins;
  font-style: normal;
  font-weight: normal;
  font-size: 18px;
  line-height: 27px;

  color: #ffffff;
  padding-top:25px;
  padding-bottom:70px
}
.container-btn {
  padding: 0;
  margin: 0;
}
.btn-get-started {
  width: 157px;
  height: 54px;
  border-radius: 100px;
  padding: 0;
  margin: 0;
  
}
</style>
