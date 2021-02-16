<template>
  <v-app>
    <router-view />
  </v-app>
</template>

<script>
export default {
  name: "App",
  mounted() {
    const html = document.querySelector("html");
    const fontSize = Math.min(50, window.innerWidth / 10);
    html.style.fontSize = fontSize + "px";
  },
};
</script>

<style lang="scss" scoped>
#app {
  width: 100%;
  height: 100%;
  overflow: hidden;
}
</style>
