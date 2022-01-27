<template>
  <aside class="aside-container">
    <div class="elements-aside">
      <div>
        <a href="#"
          ><img src="@/assets/icons/documento.png" alt="documentoIconPNG"
        /></a>
      </div>
      <div>
        <a href="#"
          ><img src="@/assets/icons/search.png" alt="searchIconPNG"
        /></a>
      </div>
      <div>
        <a href="#"><img src="@/assets/icons/git.png" alt="gitIconPNG" /></a>
      </div>
      <div>
        <a href="#"
          ><img src="@/assets/icons/antivirus.png" alt="antiIconPNG"
        /></a>
      </div>
      <div>
        <a href="#"
          ><img src="@/assets/icons/extension.png" alt="extensionIconPNG"
        /></a>
      </div>
    </div>
    <div class="config-user">
      <div>
        <a href="#"><img src="@/assets/icons/user.png" alt="userIconPNG" /></a>
      </div>
      <div>
        <a href="#"
          ><img src="@/assets/icons/setting.png" alt="setttingIconPNG"
        /></a>
      </div>
    </div>
  </aside>
</template>

<script>
export default {};
</script>

<style scoped>
img {
  width: 30px;
  height: 30px;
}
.aside-container {
  background: #282a36;
  min-width: 60px;
  max-width: 60px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  padding: 10px;
}
.elements-aside {
  height: 250px;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
}
.config-user {
  height: 100px;
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  margin-bottom: 10px;
}
</style>
