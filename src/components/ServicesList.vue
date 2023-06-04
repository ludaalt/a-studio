<template>
  <ul class="services-list">
    <ServiceCard
      v-for="item in services"
      v-bind:key="item.key"
      v-bind:item="item"
      v-bind:class="item.key"
    />
  </ul>
</template>

<script>
import ServiceCard from "./ServiceCard";

export default {
  components: { ServiceCard },

  data() {
    return {
      services: [
        {
          key: "business",
          title: "Business Idea Planning",
          description:
            "We present you a proposal and discuss niffty-gritty like",
        },

        {
          key: "development",
          title: "Development Website and App",
          description: "Communication protocols apart from engagement models",
        },

        {
          key: "financial",
          title: "Financial Planning System",
          description: "Protocols apart from aengage models, pricing billing",
        },

        {
          key: "market",
          title: "Market Analysis Project",
          description: "Protocols apart from aengage models, pricing billing",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.services-list {
  position: relative;
  min-height: 100px;
  border: 3px solid purple;

  display: grid;
  gap: 30px;

  grid-template:
    "a b"
    "c d";

  li:nth-child(1) {
    grid-area: a;
    margin-top: 80px;
  }

  li:nth-child(4) {
    grid-area: d;
    margin-top: -80px;
  }

  &::after {
    position: absolute;
    z-index: -2;
    content: "";
    width: 1147px;
    height: 619px;
    background-color: #f4f9ff;
    border-top-left-radius: 150px;
    top: 0;
    left: -214px;
  }
}
</style>
