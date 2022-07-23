<template>
  <h2>UserName: {{ name }}</h2>
  <h3>Age: {{ age }}</h3>
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      required: true,
    },
    age: {
      type: Number,
      required: true,
    },
  },
  data() {
    return {};
  },
};
</script>

<style></style>
