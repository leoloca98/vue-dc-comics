<template>
  <div id="content">
    <div class="container">
      <div class="d-flex">
        <span class="text-white fs-25">Content Goes Here</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Content",
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";
#content {
  height: 120px;
  width: 100%;
  background-color: $Content-Color;
}
</style>