<template>
  <div>
    <input 
      type="text"
      @input="onInput"
    >
  </div>
</template>

<script>
export default {
  name: "SearchBar",

  methods: {
    onInput(event) {
      this.$emit("termChange", event.target.value);
    }
  }
};
</script>

<style scoped>
  input {
    width: 75%;
  }

  div {
    margin: 20px;
    text-align: center;
  }
</style>
