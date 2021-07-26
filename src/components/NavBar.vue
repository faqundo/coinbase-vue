<template>
  <div class="center examplex">
    <vs-navbar
      center-collapsed
      v-model="active"
      target-scroll="#padding-scroll-content"
    >
      <template #left>
        <img :src="logo" alt="" />
      </template>
      <vs-navbar-item :active="active == 'guide'" id="guide">
        Home
      </vs-navbar-item>
      <vs-navbar-item :active="active == 'docs'" id="docs">
        About Us
      </vs-navbar-item>
      <vs-navbar-item :active="active == 'components'" id="components">
        Blog
      </vs-navbar-item>
      <vs-navbar-item :active="active == 'license'" id="license">
        Contact Us
      </vs-navbar-item>
      <vs-navbar-item :active="active == 'license'" id="license">
        Sell Bitcoin/ Gifcards
      </vs-navbar-item>

      <template #right>
        <vs-button shadow :active="btnActive == 1" @click="btnActive = 1">
          <img :src="login" alt="" />
        </vs-button>
      </template>
    </vs-navbar>
  </div>
</template>

<script>
import logo from "@/assets/LogoCoinbase.png";
import login from "@/assets/Login.png";

export default {
  name: "NavBar",

  data: () => ({
    logo: logo,
    login: login,
    active: "guide",
    btnActive: 0,
    items: [
        { title: 'Click Me' },
        { title: 'Click Me' },
        { title: 'Click Me' },
        { title: 'Click Me 2' },
      ],
      closeOnContentClick: true,
  }),
};
</script>

<style scoped>
.center.examplex {
  padding: 20px;
  margin: 30px;
}
</style>
