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
          <div class="item-file" @click="() => (itemFile = !itemFile)">
            <span><img src="../../assets/icons/angulo.png" alt="" /></span>
            <div class="icon-file">
              <img src="@/assets/icons/open-folder.png" alt="" />
            </div>
            <div><a href="#">node_modules</a></div>
          </div>
          <div class="item-file">
            <span><img src="../../assets/icons/angulo.png" alt="" /></span>
            <div class="icon-file">
              <img src="@/assets/icons/open-folder.png" />
            </div>
            <div><a href="#">public</a></div>
          </div>
          <div class="item-file">
            <span><img src="../../assets/icons/angulo.png" alt="" /></span>
            <div class="icon-file">
              <img src="@/assets/icons/open-folder.png" />
            </div>
            <div><a href="#">src</a></div>
          </div>
          <div class="item-file">
            <span><img src="../../assets/icons/angulo.png" alt="" /></span>
            <div class="icon-file">
              <img src="@/assets/icons/open-folder.png" />
            </div>
            <div><a href="#">.gitignore</a></div>
          </div>
          <div class="item-file">
            <span><img src="../../assets/icons/angulo.png" alt="" /></span>
            <div class="icon-file">
              <img src="@/assets/icons/open-folder.png" />
            </div>
            <div><a href="#">package-lock.json</a></div>
          </div>
          <div class="item-file">
            <span><img src="../../assets/icons/angulo.png" alt="" /></span>
            <div class="icon-file">
              <img src="@/assets/icons/open-folder.png" />
            </div>
            <div><a href="#">package.json</a></div>
          </div>
          <div class="item-file">
            <span><img src="../../assets/icons/angulo.png" alt="" /></span>
            <div class="icon-file">
              <img src="@/assets/icons/open-folder.png" />
            </div>
            <div><a href="#">README.md</a></div>
          </div>
          <div class="item-file">
            <span><img src="../../assets/icons/angulo.png" alt="" /></span>
            <div class="icon-file">
              <img src="@/assets/icons/open-folder.png" />
            </div>
            <div><a href="#">lorem</a></div>
          </div>
        </div>
      </div>
    </div>
    <div class="container-npm-scripts">
      <div class="items-npm-scripts">
        <div :style="{ color: setInputColorTrue }" v-if="setInputAnimation">
          <span
            ><img src="../../assets/icons/angulo.png" alt="" /> npm
            scripts</span
          >
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
      itemFile: false,
    };
  },
  methods: {},

};
</script>

<style scoped>
.containerExplorer {
  min-width: 250px;
  display: grid;
  background: #21222c;
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
  padding: 5px;
}
.container-row-files {
  display: flex;
  flex-direction: column;
}
.container-row-files div {
  margin: 1px;
  /* background: rgba(240, 227, 227, 0.11); !important*/
}
.container-row-files div:hover {
  transition: 0.3s;
  background: #44475a70;
}
.item-file {
  display: flex;
  align-self: stretch;
  align-items: center;
}
.item-file span img {
  width: 9px;
  height: 9px;
  transform: rotate(91deg);
}
.icon-file img {
  width: 20px;
  height: 20px;
}
</style>
