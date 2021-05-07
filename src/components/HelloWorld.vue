<template>
  <div class="hello">
    <link rel="stylesheet"
        href="https://use.fontawesome.com/releases/v5.2.0/css/all.css"
        integrity="sha384-hWVjflwFxL6sNzntih27bfxkr27PmbbK/iSvJ+a4+0owXq79v+lsFkW54bOGbiDQ"
        crossorigin="anonymous">
    <div class="desc">
    <h1>{{ msg }}</h1>
    <h3>
      Estudiante de Licenciatura en Informática
    </h3>
    <h4>Analista de Calidad de Software @Infosis.com.ar</h4>
    </div>

    <div class="icons">
    <a href="https://github.com/JuanGiacalone"><i class="fab fa-github fa-3x"></i></a>
    <a href="https://www.linkedin.com/in/juan-pablo-giacalone-478b77172/"><i class="fab fa-linkedin fa-3x"></i></a>
    <a href="https://t.me/juangia97"><i class="fab fa-telegram fa-3x"></i></a>
    </div>

  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h1{
  padding: 0.5vh;
}
h4 {
  margin: 1vw;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
i{
  margin: 2vw;
}
a {
  color: inherit;
}
a:hover{
  color: grey;
  transform: scale(1.10);
  transition: transform .25s;
  -o-transform: scale(1.10);
}
</style>
