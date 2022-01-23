<template>
  <div class="grid container">
    <div class="containerFlex select">
      <img
        src="../assets/VisualStudioCode_icon.svg.png"
        alt="visualStudioCodeIcon"
        class="visualStudioCodeIcon"
      />
      <a>File</a>
      <a>Edit</a>
      <a>Selection</a>
      <a>View</a>
      <a>Go</a>
      <a>Run</a>
      <a>Terminal</a>
      <a>Help</a>
    </div>
    <div class="containerFlex visual">
      <a href="">lorem lorem lorem</a>
    </div>
    <div class="containerFlex options-header">
      <a>icon</a>
      <a>File</a>
      <a>Edit</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>
<style>
.visualStudioCodeIcon {
  width: 20px;
  height: 20px;
}
.grid {
  width: 100%;
  height: 4vh;
  background: #282a36;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
}
.containerFlex {
  display: flex;
  align-items: center;
}
.select {
  flex-wrap: nowrap;
  justify-content: space-between;
}
.visual {
  flex-wrap: nowrap;
  text-align: center;
}

.options-header {
  width: auto;
  height: auto;
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
/* Extra small devices (phones, 600px and down)
@media only screen and (max-width: 600px) {...}

/* Small devices (portrait tablets and large phones, 600px and up) */
@media only screen and (max-width: 600px) {
  .grid {
   grid-template-columns: repeat(2, 1fr);
  }
}

/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (max-width: 768px) {
  .grid {
    grid-template-columns: repeat(2, 1fr);
  }
  .visual {
    display: none;
  }
   .options-header a { 
    margin-left: auto;
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