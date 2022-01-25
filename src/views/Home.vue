<template>
  <div class="home">
    <Header />
    <div class="grid containerHome">
      <Aside />
      <Explorer />
      <Plataform />
    </div>
  </div>
</template>

<script>
import Header from "@/components/header/Header.vue";
import Aside from "@/components/aside/Aside.vue";
import Explorer from "@/components/explorer/Explorer.vue";
import Plataform from "@/components/plataform/Plataform.vue";

export default {
  name: "Home",
  components: {
    Header,
    Aside,
    Explorer,
    Plataform,
  },
};
</script>

<style>
.grid {
  display: grid;
  grid-template-columns: 50px 250px 1fr;
}
.home {
  width: 100%;
  height: 100%;
}
</style>
