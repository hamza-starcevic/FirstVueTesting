<script>
import taskApp from "./taskApp.vue";
export default {
  components: { taskApp },
};
</script>

<template>
  <div id="h1">
    <h1>A list of the things you need to do, duh!</h1>
    <task-app />
  </div>
</template>

<style>
body {
  height: 100%;
}
#h1,
h1 {
  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px,
    rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px,
    rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
  width: 70%;
  background-color: rgba(223, 238, 181, 0.972);
  padding-top: 0.5em;
  margin-top: 0px;
  margin-left: 15%;
  height: 100%;
}
h1 {
  height: auto;
  box-shadow: none !important;
}
</style>
>
