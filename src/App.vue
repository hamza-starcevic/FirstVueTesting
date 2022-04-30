<script>
import MiddleContent from "./components/middleContent.vue";
import topBar from "./components/topBar.vue";
export default {
  components: { topBar, MiddleContent },
};
</script>

<template>
  <top-bar />
  <middle-content />
</template>

<style>
body,
html {
  overflow: hidden;
  width: 100%;
  height: 100%;
  background-color: rgb(152, 176, 111);
}
#app {
  height: 100%;
}
</style>
