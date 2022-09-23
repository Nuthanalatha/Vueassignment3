<template>
  <h1>Example for ChildToParent and PropsValidation</h1>
  <button @click="childData">Send data1</button>
</template>

<script>
export default {
  emits: ["idData"],
  data() {
    return {
      id: 22,
    };
  },
  methods: {
    childData() {
      this.$emit("idData", this.id);
    },
  },
};
</script>

<style></style>
