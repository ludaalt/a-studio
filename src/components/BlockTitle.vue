<template>
  <div>
    <h2 class="block-title">{{ title }}</h2>
    <p class="block-description">{{ description }}</p>
  </div>
</template>

<script>
export default {
  name: "BlockTitle",
  props: {
    title: {
      type: String,
      required: true,
    },

    description: {
      type: String,
      required: true,
    },
  },
};
</script>

<style>
.block-title {
  margin-bottom: 40px;
  font-weight: 400;
  font-size: 40px;
  line-height: 49px;

  color: #000000;
}

.block-description {
  margin-bottom: 30px;
  max-width: 470px;
  text-align: start;
}
</style>
