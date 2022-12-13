<template>
  <div class="hello">
    <h1>Conversor a dólares</h1>
    Ingrese monto $ <input type="text" v-model="pesos">
    <br><br>
    Valor del dolar en $ <input type="text" v-model="dolares"> 
    <br>
    <p>Valor convertido U$D: {{calcularConversion()}}</p>
    <p>
      Respuestas: 1: C, 2: B, 3: D, 4: A, 5: C
    </p>
  </div>
</template>

<script lang="js">


export default {
    name: "src-components-final",
    props: [],
    mounted () {

    },
    data () {
        return {
            pesos: 1000,
            dolares: 312,
        }
    },
    methods: {
        calcularConversion() {
            let pesos = this.pesos;
            let dolares = this.dolares;
            let total = pesos/dolares;
            return total;
        }
    },
    
}
</script>

<style >

</style>
