<template>
  <h1>Example for ChildToParent and PropsValidation</h1>
  <button @click="childData">Send data4</button>
</template>

<script>
export default {
  emits: ["subData"],
  data() {
    return {
      sub: "1-5",
    };
  },
  methods: {
    childData() {
      this.$emit("subData", this.sub);
    },
  },
};
</script>

<style></style>
