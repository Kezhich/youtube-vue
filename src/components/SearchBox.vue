<template>
  <div>
    <input @input="onInput">
  </div>
</template>

<script>
export default {
  name: "searchbox",
  methods: {
    onInput: function(e) {
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
  text-align: center;
  margin: 20px;
}
</style>
