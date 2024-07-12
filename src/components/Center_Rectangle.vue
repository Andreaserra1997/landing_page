<script>
export default {};
</script>

<template>
  <div class="rectangle">
    <div class="brown-square"></div>
    <div class="white-square"></div>
    <div class="azure-square"></div>
  </div>
</template>

<style>
.rectangle {
  display: flex;
}
.brown-square,
.azure-square {
  width: 25%;
  height: calc((100vh / 3) - 36.66px);
}
.white-square {
  width: 50%;
  background-image: url(/Mosaic.png);
  background-repeat: no-repeat;
  background-position: center;
}
.brown-square {
  background-color: #c19e84;
}
.white-square {
  background-color: white;
}
.azure-square {
  background-color: #c19e84;
}
</style>
