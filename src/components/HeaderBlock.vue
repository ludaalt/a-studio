<template>
  <NavigationPanel />
  <div class="description-block">
    <div class="page-container title-block">
      <BlockTitle
        title="A Digital Product Agency"
        description="Leading digital agency with solid design and development expertise. We
        build readymade websites, mobile applications, and elaborate online
        business services."
      />
      <AppButton title="Contact Now" />
    </div>
    <picture>
      <img src="../assets/team.png" alt="Our team" />
    </picture>
  </div>
</template>

<script>
import BlockTitle from "./BlockTitle";
import NavigationPanel from "./NavigationPanel";
import AppButton from "./AppButton.vue";

export default {
  name: "HeaderBlock",
  components: { BlockTitle, NavigationPanel, AppButton },
};
</script>

<style scoped lang="scss">
.description-block {
  display: flex;
  max-width: 1770px;
  margin: 0 auto;

  picture {
    margin-left: auto;
    position: relative;

    &::before,
    &::after {
      z-index: -1;
      position: absolute;
      content: "";
    }

    &::before {
      width: 129px;
      height: 129px;
      left: -70px;
      top: 0;
      border-radius: 50%;
      background: #dae9ff;
    }

    &::after {
      width: 178px;
      height: 178px;

      right: 120px;
      bottom: -80px;
      border-bottom-right-radius: 100px;
      background: #fff5db;
    }
  }

  img {
    border-bottom-left-radius: 30%;
    object-fit: cover;
    width: 755px;
    height: 512px;
    filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.25));
  }

  .title-block {
    padding: 125px 0;
  }
}
</style>
