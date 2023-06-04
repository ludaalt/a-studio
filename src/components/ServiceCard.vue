<template>
  <li>
    <div class="icon-block">
      <img
        :src="require(`../assets/services/${item.key}.svg`)"
        :alt="item.key"
      />
    </div>
    <h3>{{ item.title }}</h3>
    <p>{{ item.description }}</p>
  </li>
</template>

<script>
export default {
  name: "ServiceCard",
  props: {
    item: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style scoped>
li {
  padding: 40px 30px 50px;
  background-color: #fff;
  width: 308px;
  height: 379px;

  border: 1px solid #f2f2f2;
  box-shadow: 0px 10px 50px rgba(0, 0, 0, 0.05);
  border-radius: 40px;
}

.icon-block {
  margin: 0 auto;
  width: 121px;
  height: 121px;
  border-radius: 20px;
  display: flex;
  align-items: center;
  justify-content: center;
}

li.business > .icon-block {
  background-color: #f1f7ff;
}

h3 {
  margin: 30px 0;
  max-width: 240px;
  font-weight: 400;
  font-size: 24px;
  line-height: 30px;
  text-align: center;
  color: #000;
}

p {
  /* font-family: 'Averta Demo PE Cutted Demo'; */

  font-weight: 400;
  font-size: 16px;
  line-height: 140%;

  text-align: center;

  color: #757575;
}
</style>
