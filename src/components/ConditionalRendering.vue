<template>
  <button @click="awesome = !awesome">toggle</button>
  <h1 v-if="awesome">Vue is awesome!</h1>
  <h1 v-else>on no😒</h1>
</template>

<script>
export default {
  data() {
    return {
      awesome: true,
    };
  },
};
</script>

<style></style>
