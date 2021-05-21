<template>
  <div class="circle"></div>
</template>

<script>
export default {
  name: "Circle",
  props: {},
};
</script>

<style scoped>
.circle {
  width: 35px;
  height: 35px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: all 0.2s ease-out;
  margin: 22px;
}
.circle:hover {
  width: 50px;
  height: 50px;
}
</style>
