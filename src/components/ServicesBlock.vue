<template>
  <div class="page-container services">
    <BlockTitle
      title="How can we help your Business ?"
      description="We build readymade websites, mobile applications, and elaborate online business services."
    />
    <ServicesList />
  </div>
</template>

<script>
import BlockTitle from "./BlockTitle";
import ServicesList from "./ServicesList";

export default {
  components: { BlockTitle, ServicesList },
};
</script>

<style lang="scss">
div.services {
  border: 3px solid red;
  margin-bottom: 146px;
  display: flex;
  justify-content: space-between;
  align-items: center;

  .block-title {
    max-width: 358px;
    //posi
  }

  .block-description {
    max-width: 396px;
  }
}
</style>
