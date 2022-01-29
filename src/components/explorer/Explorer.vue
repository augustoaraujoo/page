<template>
  <div class="containerExplorer">
    <div class="text-explorer">
      <div>
        <a href="#"> EXPLORER</a>
      </div>

      <div>
        <span>...</span>
      </div>
    </div>
    <!--  -->
    <div class="folders-in-explorer">
      <div class="container-files">
        <div class="container-row-files">
          <div class="item-file">
            <span>></span>
            <div>📂</div>
            <div>node_modules</div>
          </div>
          <div class="item-file">
            <span>></span>
            <div>📂</div>
            <div>public</div>
          </div>
          <div class="item-file">
            <span>></span>
            <div>📂</div>
            <div>src</div>
          </div>
          <div class="item-file">
            <span>></span>
            <div>📂</div>
            <div>.gitignore</div>
          </div>
          <div class="item-file">
            <span>></span>
            <div>📂</div>
            <div>package-lock.json</div>
          </div>
          <div class="item-file">
            <span>></span>
            <div>📂</div>
            <div>package.json</div>
          </div>
          <div class="item-file">
            <span>></span>
            <div>📂</div>
            <div>README.md</div>
          </div>
          <div class="item-file">
            <span>></span>
            <div>📂</div>
            <div>lorem</div>
          </div>
        </div>
      </div>
    </div>
    <div class="container-npm-scripts">
      <div class="items-npm-scripts">
        <div :style="{ color: setInputColorTrue }" v-if="setInputAnimation">
          <span>> npm scripts</span>
        </div>
        <div v-else :style="{ color: setInputColorFalse }">⬇️ npm scripts</div>
        <button @click="() => (setInputAnimation = !setInputAnimation)">
          set
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      setInputAnimation: false,
      setInputColorFalse: "#424450",
      setInputColorTrue: "#250",
    };
  },
};
</script>

<style scoped>
.containerExplorer {
  min-width: 250px;
  display: grid;
  background: #21222C;
  grid-template-columns: 1fr;
  grid-template-rows: 40px 1fr 180px;
}
.text-explorer {
  background: #21222c;
  display: flex;
  padding: 10px;
  align-items: center;
  justify-content: space-between;
}
.text-explorer span,
a {
  color: #ffff;
}
.folders-in-explorer {
  background: #44475a70;
}
.container-npm-scripts {
  flex: 1;
}
.items-npm-scripts {
  /* background: #2436ad70; */
}
.container-files {
  /* background: #ee32; */
}
.container-row-files {
  display: flex;
  flex-direction: column;
}
.container-row-files div {
  margin: 3px;
  /* background: rgba(240, 227, 227, 0.11); !important*/
}
.item-file {
  display: flex;
  align-items: center;
}
</style>
