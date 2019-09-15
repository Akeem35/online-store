<template>
  <div>
    <h1>This is the about Page</h1>
  </div>
</template>

<script>
export default {
  async asyncData({ $axios }) {
    const res = await $axios.$get('http://localhost:5000/api/products/')
    console.log(res)
  }
}
</script>

<style>

</style>