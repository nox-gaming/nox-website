<template>
  <img src="/img/logo.png" alt="logo" />
</template>

<style>
img {
  width: calc(100% / 10);
  margin: 0 auto;
  animation-duration: 10s;
  animation: appearIn 0.6s 1 0s ease-in;
}
@-webkit-keyframes appearIn {
  from {
    top: 0px;
    opacity: 0;
  }
  to {
    top: 200px;
    opacity: 1;
  }
}
@keyframes appearIn {
  from {
    top: 0px;
    opacity: 0;
  }
  to {
    top: 200px;
    opacity: 1;
  }
}
</style>

<script>
name: 'Logo'
export default {}
</script>