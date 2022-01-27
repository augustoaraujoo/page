<template>
  <div class="grid">
    <Header class="header" />
    <Aside class="aside" />
    <Explorer class="explorer" />
    <Plataform class="plataform" />
    <Footer class="footer" />
  </div>
</template>

<script>
import Header from "@/components/header/Header.vue";
import Aside from "@/components/aside/Aside.vue";
import Explorer from "@/components/explorer/Explorer.vue";
import Plataform from "@/components/plataform/Plataform.vue";
import Footer from "@/components/footer/Footer.vue";

export default {
  name: "Home",
  components: {
    Header,
    Aside,
    Explorer,
    Plataform,
    Footer,
  },
};
</script>

<style>
.grid {
  width: 100%;
  height: 100vh;
  display: grid;
  grid-template-columns: 60px 250px 1fr;
  grid-template-rows: auto 1fr;
  grid-column-gap: 0px;
  grid-row-gap: 0px;
}

.header {
  grid-area: 1 / 1 / 2 / 6;
}
.aside {
  grid-area: 2 / 1 / 6 / 2;
}
.explorer {
  grid-area: 2 / 2 / 6 / 3;
}
.plataform {
  grid-area: 2 / 3 / 6 / 6;
}
.footer {
  grid-area: 5 / 1 / 6 / 6;
}
</style>
