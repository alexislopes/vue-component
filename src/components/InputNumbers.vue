<template>
  <div id="one">
    <input type="number" :value='one' @blur='pegar_one' placeholder="Digite o 1º número">
    <input type="number" :value='two' @blur='pegar_two' placeholder="Digite o 2º número">
  </div>
</template>

<script>
export default {
  name: "InputNumbers"
};

data(){
    methods: {
        pegar_one(event){
            
        }
    }
}
</script>

