<script>
export default {};
</script>

<template>
  <div class="rectangle">
    <div class="light_blue-square effect3"></div>
    <div class="violet-square"></div>
    <div class="green-square"></div>
    <div class="water-square effect4"></div>
  </div>
</template>

<style>
.rectangle {
  display: flex;
}
.light_blue-square,
.violet-square,
.green-square,
.water-square {
  width: 25%;
  height: calc((100vh / 3) - 36.66px);
}
.effect3,
.effect4 {
  backdrop-filter: blur(7px);
  transition: all 0.3s;
  cursor: pointer;
}

.effect3:hover {
  box-shadow: 35px 35px 68px 0px rgba(157, 188, 255, 0.5);
}
.effect4:hover {
  box-shadow: 35px 35px 68px 0px rgba(11, 233, 229, 0.445);
}

.effect3:active,
.effect4:active {
  transform: scale(0.95);
}

.effect3:active {
  border: 1px solid blue;
}
.effect4:active {
  border: 1px solid lightskyblue;
}
.light_blue-square {
  background-color: #055c68;
  background-image: url(/Plumen.png);
  background-repeat: no-repeat;
  background-position: center;
}
.violet-square {
  background-color: #4d3d50;
}
.green-square {
  background-color: #84c1ac;
}
.water-square {
  background-color: #8bcce0;
  background-image: url(/EIVA.png);
  background-repeat: no-repeat;
  background-position: center;
}
</style>
