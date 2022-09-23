<template>
  <button @click="something = !something">toggle</button>
  <h1 v-if="something">Vue is something!</h1>
  <h1 v-else>on no😒</h1>
</template>

<script>
export default {
  data() {
    return {
      something: false,
    };
  },
};
</script>

<style></style>
