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

<style scoped>
#content {
  height: 120px;
  width: 100%;
  background-color: rgb(28, 28, 28);
}

.d-flex {
  height: 120px;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: start;
}

.fs-25 {
  font-size: 25px;
}
</style>