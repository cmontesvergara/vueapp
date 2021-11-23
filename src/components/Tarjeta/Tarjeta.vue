<template>
<div class="cuerpo">
    <img :src="ruta" alt="">
    <h3>{{titulo}}</h3>
    <p>{{parrafo}}</p>
    <button>Click me</button>
</div>
</template>

<script>
export default {
name:"Tarjeta",
data: function(){
    return{
        titulo: "Soy el titulo",
        ruta: "/path/..",
        parrafo: "Soy el Parrafo",
        boton: "",
    }
}
}
</script>

<style scoped>
.cuerpo{
    display: flex;
    flex-direction: column;
    width: 200px;
    height: 300px;
    margin: 10px;
    padding: 5px;
    box-shadow: 0px 0px 7px rgba(65, 0, 65, 0.514);
    border-radius: 5px;
}

</style>