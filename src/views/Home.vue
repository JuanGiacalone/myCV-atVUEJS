<template>
  <div class="card">
    <img alt="me" class="me" src="../assets/me.jpg">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue';

export default {
  name: 'Home',
  components: {
    HelloWorld,
  },
};
</script>
<style scoped>
@import url("https://fonts.googleapis.com/css?family=Tajawal:300,400");
.card {
  width: 60vw;
    height:60vh;
    background: linear-gradient(to right, #eb3349, #f45c43);
    font-family: 'Tajawal', sans-serif;
    box-shadow: 1px 2px 10px grey;
    /* center itself */
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
    /* center its children */
    display: flex;
    align-items: center;
    justify-content: center;
}
.me {
  height: 40vh;
  border-radius: 5%;
  margin: 1vw;
  z-index: 1;
  border: 0.5vw;
  box-shadow:  5px 8px 6px -6px black;;
};
.me:hover img {
  transition: transform .25s ease;
  transform:  scale(.5);
}
</style>
