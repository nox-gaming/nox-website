<template>
  <div id="page">
    <Header />
    <Community />
  </div>
</template>

<script>
import Header from '@/components/Index/Header'
import Community from '@/components/Index/Community'

export default {
  components: {
    Header,
    Community
  }
}
</script>

<style>
#page {
  display: flex;
  flex-direction: column;
}
section {
  display: flex;
  flex-direction: column;
  top: 0;
  left: 0;
  width: 100%;
  height: 100vh;
  text-align: center;
  color: white;
  overflow-y: hidden;
}
</style>
