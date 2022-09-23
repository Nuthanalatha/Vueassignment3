<template>
  <h1>{{ greeting }}</h1>
</template>

<script>
export default {
  props: {
    greeting: {
      type: String,
      required: true,
    },
  },
};
</script>

<style></style>
