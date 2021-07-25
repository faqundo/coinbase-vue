<template>
  <div>
    <v-app-bar flat dense prominent>
      <v-img
        lazy-src="https://picsum.photos/id/11/10/6"
        max-height="28"
        max-width="142"
        :src="logo"
      ></v-img>

    </v-app-bar>
  </div>
</template>

<script>
import logo from "@/assets/LogoCoinbase.png";

export default {
  name: "NavBar",

  data: () => ({
      logo:logo
  }),
};
</script>
