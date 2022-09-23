<template>
  <h1>Example for ChildToParent and PropsValidation</h1>
  <button @click="childData">Send data</button>
</template>

<script>
export default {
  emits: ["add"],
  data() {
    return {
      name: "nuthana",
    };
  },
  methods: {
    childData() {
      this.$emit("add", this.name);
    },
  },
};
</script>

<style></style>
