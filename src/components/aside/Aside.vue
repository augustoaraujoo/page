<template>
  <aside class="aside-container">
    <div class="elements-aside">
      <div>
        <a href="#"
          ><img src="@/assets/icons/documento.png" alt="documentoIconPNG"
        /></a>
      </div>
      <div @click="search" class="searchIconContainer">
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
export default {
  data() {
    return {
      inputSearch:''
    }
  },
  computed: {
    
  },
};
</script>

<style scoped>
.searchIconContainer img {
  transform: scaleX(-1);
}
img {
  width: 30px;
  height: 30px;
  filter: contrast(50%);
}
img:hover {
  filter: contrast(5%);
}
.aside-container {
  background: #191a21;
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
  justify-content: space-between;
}
.config-user {
  height: 100px;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  margin-bottom: 10px;
}
</style>
