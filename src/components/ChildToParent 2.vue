<template>
  <h1>Example for ChildToParent and PropsValidation</h1>
  <button @click="childData">Send data2</button>
</template>

<script>
export default {
  emits: ["ageData"],
  data() {
    return {
      age: "22",
    };
  },
  methods: {
    childData() {
      this.$emit("ageData", this.age);
    },
  },
};
</script>

<style></style>
