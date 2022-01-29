<template>
  <div class="container">
    <nav class="container-nav">Lorem</nav>
    <div class="container-section">Lorem</div>
    <div class="container-terminal">Lorem</div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.container {
  display: grid;
  grid-template-rows: 40px 1fr 200px;
  background: #1b1c24fb;
}
.container-nav {
  background: #1b1c24;
  padding: 10px;
  display: flex;
  align-items: center;
}
.container-terminal {
  background: #1b1c24b2;
}
</style>
