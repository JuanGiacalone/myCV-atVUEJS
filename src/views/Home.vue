<template>
  <div class="card">
    <div
    class="img-div">
      <img  alt="me" class="me" src="../assets/me.jpg">
    </div>
    <HelloWorld msg="Juan Pablo Giacalone"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue';

export default {
  name: 'Home',
  data() {
    return {
      hover: false,
    };
  },
  components: {
    HelloWorld,
  },
};
</script>
<style scoped>
@import url("https://fonts.googleapis.com/css?family=Tajawal:300,400");

.card {
  width: 70vw;
    height:70vh;
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
  border-radius: 5.5%;
  margin: 5vw;
  margin-left: 2vw;
  z-index: 1;
  border: 0.5vw;
  box-shadow:  8px 8px 6px -6px black;
};
.img-div:hover {
  transition: transform .25s;
  transform:  scale(1.20);
}
</style>
