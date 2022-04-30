<script>
export default {};
</script>

<template>
  <div id="main">
    <div id="left">Todo App</div>
    <div id="right">Login</div>
  </div>
</template>

<style>
#main {
  box-shadow: rgba(6, 24, 44, 0.4) 0px 0px 0px 2px,
    rgba(6, 24, 44, 0.65) 0px 4px 6px -1px,
    rgba(255, 255, 255, 0.08) 0px 1px 0px inset;
  display: flex;
  color: rgb(68, 43, 72);
  font-weight: 900;
  font-size: 1.5em;
  background-color: #ffdc00;
  position: relative;
  width: 100%;
  height: 4rem;
  line-height: 4rem;
}

#left,
#right {
  padding-left: 4em;
  width: 50%;
}
li {
  font-size: 2em;
}
body {
  margin: 0px;
  width: 100%;
}
</style>
