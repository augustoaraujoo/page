<template>
  <div class="container">
    <div class="containerFlex select">
      <div>
        <img
          src="../../assets/icons/VisualStudioCode_icon.svg.png"
          alt="visualStudioCodeIcon"
          class="visualStudioCodeIcon"
        />
        <a href="#">File</a>
        <a href="#">Edit</a>
        <a href="#">Selection</a>
        <a href="#">View</a>
        <a href="#">Go</a>
        <a href="#">Run</a>
        <a href="#">Terminal</a>
        <a href="#">Help</a>
      </div>
    </div>

    <div class="containerFlex visual">
      <a href="" id="info-profile">this is my profile :)</a>
    </div>

    <div class="containerFlex options-header">
      <img src="../../assets/icons/negativeIcon.png" alt="" class="icon" />
      <img src="../../assets/icons/422371.svg" alt="" class="icon" />
      <img src="../../assets/icons/img_333885.png" alt="" class="icon" />
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>
<style scoped>
a {
  filter: contrast(100%);
  color: #f8f8f2;
}
.icon {
  width: 15px;
  height: 15px;
  filter: contrast(5%);
}
.visualStudioCodeIcon {
  width: 20px;
  height: 20px;
  margin-left: 5px;
}
.container {
  height: 30px;
  padding: 5px;
  display: flex;
  align-items: center;
  flex-wrap: nowrap;
  background: #191a21;
}
.containerFlex {
  display: flex;
  align-items: center;
}
.select {
  min-width: 500px;
  max-width: 600px;
  margin-right: auto;
}
.select > div {
  flex: 1;
  display: flex;
  flex-wrap: nowrap;
  align-items: center;
  justify-content: space-around;
}
.select a:hover {
  filter: contrast(10%);
  transition: 0.3s;
}
.visual {
  display: inline;
}

.options-header {
  margin-left: auto;
  width: 100px;
  display: flex;
  align-items: center;
  justify-content: space-around;
}

li {
  list-style-type: none;
  /* - &BG       '#282A36'
    - &FG        '#F8F8F2'
    - &SELECTION '#44475A'
    - &COMMENT   '#6272A4'
    - &PINK      '#FF79C6'
    - &PURPLE    '#BD93F9'
  ansi:
    - &COLOR0    '#21222C'
    - &COLOR7    '#F8F8F2'
    - &COLOR8    '#6272A4' 
    - &LineHighlight '#44475A75'
    - &NonText       '#FFFFFF1A'
    - &WHITE         '#FFFFFF'
    - &TAB_DROP_BG   '#44475A70'
    # UI Variants
    - &BGLighter     '#424450'
    - &BGLight       '#343746' # HSV (230   , 25.71, 27.45)
    - &BGDark        '#21222C' # HSV (234.55, 25   , 17.25)
    - &BGDarker      '#191A21' # HSV (234.55, 25   , 13   )*/
}

/* Small devices (portrait tablets and large phones, 600px and up) */
@media only screen and (max-width: 600px) {
  .select {
    min-width: auto;
  }
  .select > div {
    min-width: auto;
  }
}

/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (max-width: 768px) {
  .select {
    min-width: 310px;
  }
  .visual {
    display: none;
  }
  .options-header {
    margin-left: auto;
  }
}

/* Large devices (laptops/desktops, 992px and up) */
/*@media only screen and (max-width: 992px) {...}*/

/* Extra large devices (large laptops and desktops, 1200px and up) */
/*@media only screen and (max-width: 1200px) {...}*/
</style>
