<template>
  <nav>
    <div class="content-navbar">
      <ul>
        <li><h1>Brand</h1></li>
        <li>Productos</li>
        <li>Personas</li>
      </ul>
    </div>
    <div class="content-navbar">
      <ul>
        
        <li v-if="!logueado">Iniciar Sesion</li>
        <li v-if="logueado">Cerrar Sesion</li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: "NavBar",
  data:function() {
      return {
        logueado: false
      }
  }
};
</script>

<style scoped>
.content-navbar {
  display: flex;
}
nav {
  display: flex;
  justify-content: space-between;
  width: 100vw;
  height: 60px;
  background: rgba(158, 22, 158, 0.856);
  box-shadow: 1px 2px 10px rgb(126, 125, 125);
}
ul {
  display: flex;
  width: 100%;
  height: 100%;
  justify-content: flex-start;
  align-items: center;
  margin: 0px;
}
li {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 5px;
}
</style>
