<template>
  <div class="data-box">
    {{ title }}
  </div>
</template>

<script>
export default {
  name: "Box",
  props: {
    title: String,
  },
  data() {
    return {};
  },
};
</script>

<style scoped>
.data-box {
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 16px;
  margin: 0 8px 8px 0;
  padding: 15px 20px;
  height: 45px;
  border-radius: 6px;
  border: 1px solid #dfdede;
  cursor: pointer;
}

.data-box:hover {
  border-color: #099688;
}
</style>
