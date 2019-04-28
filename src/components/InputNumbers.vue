<template>
  <div>
    <input type="number" :value="one" @input="getFirstNumber" placeholder="Digite o 1º número">
    <input
      type="number"
      :value="two"
      @input="getSecondNumber"
      v-on:input="$emit('input', $event.target.value)"
      placeholder="Digite o 2º número"
    >
  </div>
</template>

<script>
export default {
  name: "input",

  data: function() {
    return {
      one: 0,
      two: 0
    };
  },
  methods: {
    getFirstNumber(event) {
      this.one = event.target.value;
      this.$emit("sendOne", this.one);
    },

    getSecondNumber(event) {
      this.two = event.target.value;
      this.$emit("sendTwo", this.two);
    }
  }
};
</script>

