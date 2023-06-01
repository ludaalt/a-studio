<template>
  <div class="page-container navigation-panel-container">
    <a href="#" class="main-logo"></a>

    <nav>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">What We Do</a></li>
        <li><a href="#">Service</a></li>
        <li><a href="#">Project</a></li>
        <li><a href="#">Blog</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
.navigation-panel-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.main-logo {
  display: inline-block;
  width: 120px;
  height: 34px;
  background: url("../assets/main-logo.svg") no-repeat center;
}

ul {
  display: flex;
  padding: 20px 0;

  li {
    a {
      display: inline-block;
      padding: 20px 10px;

      &:hover {
        text-decoration: underline;
      }
    }
  }

  li:not(:last-child) {
    margin-right: 40px;
  }
}
</style>
