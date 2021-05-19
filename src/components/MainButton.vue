<template>
  <button @click="nextSection">
    {{ content }}
  </button>
</template>

<script>
export default {
  name: "MainButton",
  props: {
    content: String,
  },
  data() {
    return {};
  },
  methods: {
    nextSection() {},
  },
};
</script>

<style scoped>
button {
  border-radius: 3px;
  background-color: #705eeb;
  color: #fff;
  padding: 0 30px;
  height: 48px;
  text-align: center;
  text-decoration: none;
  font-size: 16px;
  cursor: pointer;
  border: none;
  font-weight: bold;
}

button:hover {
  background-color: #513be0;
}
</style>
