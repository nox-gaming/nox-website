<template>
    <div class="container">
        <h1 v-if="error.status === 404">Page not found</h1>
        <h1 v-else>Whoopsi and error occured!</h1>
        <nuxt-link to="/">Okay let's go home</nuxt-link>
    </div>
</template>

<style scoped>
a {
    color: red;
}
</style>

<script>
export default {
    props: ['error']
}
</script>