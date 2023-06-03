<template>
  <div class="page-container clients">
    <BlockTitle
      title="Our Client"
      description="Several selected clients, who already believe in our service."
    />

    <ul>
      <li v-for="client in clients" v-bind:key="client.name">
        <img
          :src="require(`../assets/clients/${client.name}.svg`)"
          :alt="client"
        />
      </li>
    </ul>
  </div>
</template>

<script>
import BlockTitle from "./BlockTitle.vue";

export default {
  name: "ClientsBlock",
  components: { BlockTitle },

  data() {
    return {
      clients: [
        { name: "google" },
        { name: "airbnb" },
        { name: "uber" },
        { name: "amazon" },
      ],
    };
  },

  computed: {
    itemImage(client) {
      return require(`../assets/clients/${client}.svg`);
    },
  },
};
</script>

<style lang="scss">
div.clients {
  margin: 130px auto 90px;
  display: flex;
  justify-content: space-between;
  align-items: center;

  .block-title {
    margin-bottom: 17px;
  }

  .block-description {
    max-width: 335px;
  }

  ul {
    display: flex;
    align-items: center;

    li:not(:last-child) {
      margin-right: 60px;
    }
  }
}
</style>
