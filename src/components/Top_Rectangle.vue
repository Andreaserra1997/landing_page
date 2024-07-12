<script>
export default {};
</script>

<template>
  <div class="rectangle">
    <div class="red-square effect1"></div>
    <div class="pink-square"></div>
    <div class="blue-square"></div>
    <div class="yellow-square effect2"></div>
  </div>
</template>

<style>
.rectangle {
  display: flex;
}
.red-square,
.pink-square,
.blue-square,
.yellow-square {
  width: 25%;
  height: calc((100vh / 3) - 36.66px);
}
.effect1,
.effect2 {
  backdrop-filter: blur(7px);
  transition: all 0.3s;
  cursor: pointer;
}

.effect1:hover {
  box-shadow: 35px 35px 68px 0px rgba(255, 169, 157, 0.5);
}
.effect2:hover {
  box-shadow: 35px 35px 68px 0px rgba(255, 252, 157, 0.5);
}

.effect1:active,
.effect2:active {
  transform: scale(0.95);
}

.effect1:active {
  border: 1px solid red;
}
.effect2:active {
  border: 1px solid yellow;
}
.red-square,
.yellow-square {
  background-repeat: no-repeat;
  background-position: center;
}
.red-square {
  background-color: #bb2649;
  background-image: url(/CreativeCables.png);
}
.yellow-square {
  background-color: #edb944;
  background-image: url(/Bebulbs.png);
}
.pink-square {
  background-color: #deb7e5;
}
.blue-square {
  background-color: #616ea3;
}
</style>
