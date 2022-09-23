<template>
  <h1>Example one for ParentToChild and PropValidation</h1>
  <h2>FullName: {{ FirstName }} {{ LastName }}</h2>
  <h2>RollNumber: {{ RollNo }}</h2>
</template>

<script>
export default {
  props: {
    FirstName: {
      type: String,
      required: true,
    },
    LastName: {
      type: String,
      required: true,
    },
    RollNo: {
      type: Number,
      default: 90,
    },
  },
};
</script>

<style></style>
