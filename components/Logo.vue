<template>
  <img src="../assets/logo.png" alt="logo" />
</template>

<style>
img {
  width: calc(100% / 10);
  margin: 0 auto;
}
@keyframes turn {
  100% {
    transform: rotateX(0deg);
  }
}

@keyframes godown {
  100% {
    top: 180px;
  }
}

@keyframes goright {
  100% {
    left: 70px;
  }
}
</style>

<script>
name: 'Logo'
export default {}
</script>