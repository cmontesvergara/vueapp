<template>
  <div class="contenedor" >
    <NavBar/>
    <Tarjeta/>
    <Tarjeta/>
    <Tarjeta/>
    <Tarjeta/>
    <Tarjeta/>
    <Tarjeta/>
    <Tarjeta/>
    <Tarjeta/>

  </div>
</template>

<script>
// @ is an alias to /src

import NavBar from "@/components/NavBar/NavBar.vue";
import Tarjeta from "@/components/Tarjeta/Tarjeta.vue";



export default {
  name: "Home",
  components: {
    
    NavBar,
    Tarjeta
  },
};
</script>

<style scoped>
.contenedor{
  justify-content: space-between;
  padding: 20px;
  display: flex;
  flex-wrap: wrap;
}
</style>
