<template>
  <footer>
    <div class="div-left">
      <div class="items-left">
        <a href="#"><img src="../../assets/icons/git.png" alt="" /></a>
        <a href="#">main*</a>
        <a href="#"><img src="../../assets/icons/reload-icon.png" alt="" /></a>
        <a href="#"><img src="../../assets/icons/circleX.png" alt="" /> 0</a>
        <a href="#"
          ><img src="../../assets/icons/warning_icon.png" alt="" />33</a
        >
      </div>
    </div>

    <div class="div-right">
      <div>lorem</div>
      <div>lorem</div>
      <div>lorem</div>
      <div>lorem</div>
      <div>lorem</div>
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style scoped>
img {
  width: 15px;
  height: 15px;
  filter: contrast(0%);
}
footer {
  flex: 1;
  display: flex;
  flex-wrap: nowrap;
  background: #191a21;
}

.div-left {
  min-width: 250px;
  flex: 1;
  display: flex;
}
.items-left {
  filter: contrast(0%);
  min-width: 200px;
  width: 250px;
  display: flex;
  justify-content: space-evenly;
  margin-right: auto;
  align-items: center;
}
.items-left a {
  display: flex;
  align-items: center;
}
.div-right {
  min-width: 100px;
  margin-left: auto;
  display: inline;
  filter: contrast(0%);
}
.div-right div {
  display: inline;
  margin: 5px;
}
</style>