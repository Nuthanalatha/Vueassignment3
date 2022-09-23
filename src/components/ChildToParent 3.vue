<template>
  <h1>Example for ChildToParent and PropsValidation</h1>
  <button @click="childData">Send data3</button>
</template>

<script>
export default {
  emits: ["addData"],
  data() {
    return {
      add: "1+5",
    };
  },
  methods: {
    childData() {
      this.$emit("addData", this.add);
    },
    // childMethod() {
    //   this.add = 1 + 5;
    // },
  },
};
</script>

<style></style>
