<template>
    <div>
        <h1>{{ msg }}</h1>
        <h2>{{ legenda }}</h2>
        <input type="text" v-model="legenda">
        <button @click="resetLegenda"> Reset Legenda</button>
    </div>
</template>

<script>
 export default {
    //O que eu recebo de entrada no componente 
    props: ['msg'],
    //Dados internos do componente
    data: function(){
       return {
        legenda: 'Estou no vue'
       }
    },
    //Metodos internos do componente
    methods:{
        resetLegenda(){
              this.legenda = 'Estou no vue'     
            }
    }
 }
</script>

<style>

</style>