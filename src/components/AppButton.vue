<template>
  <button>{{ title }}</button>
</template>

<script>
export default {
  name: "AppButton",
  props: {
    title: {
      type: String,
      required: true,
    },
  },
};
</script>

<style scoped lang="scss">
button {
  padding: 20px 40px;
  background: #2639ed;
  border-radius: 60px;
  font-weight: 400;
  font-size: 20px;
  line-height: 25px;
  letter-spacing: 0.065em;
  color: #ffffff;
  border: 0.5px solid #ffffff;

  &:hover {
    opacity: 0.8;
  }
}
</style>
