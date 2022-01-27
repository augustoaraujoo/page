<template>
  <div class="containerExplorer">
    <div class="text-explorer">
      <div>
        <a href="#"> explorer</a>
      </div>

      <div>
        <span>...</span>
      </div>
    </div>
    <!--  -->
    <div class="folders-in-explorer">
      <ul>
        <li>a</li>
        <li>a</li>
        <li>a</li>
        <li>a</li>
        <li>a</li>
        <li>a</li>
        <li>a</li>
        <li>a</li>
        <li>a</li>
        <li>a</li>
        <li>a</li>
        <li>a</li>
        <li>a</li>
      </ul>
    </div>
    <div class="container-npm-scripts">
      <p>Lorem ipsum dolor sit,</p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.containerExplorer {
  min-width: 250px;
  display: grid;
  grid-template-columns: 1fr;
  grid-template-rows: 40px 1fr 80px;
}
.text-explorer {
  background: #21222c;
  display: flex;
  padding: 10px;
  align-items: center;
  justify-content: space-between;
}
.folders-in-explorer {
  background: rgba(255, 105, 180, 0.671);
}
.container-npm-scripts {
  background: #e4e;
}
</style>
