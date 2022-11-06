<template>
  <div>
    <nuxt-link to="/users">users</nuxt-link>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  async asyncData(context) {
    const res = await context.app.$axios.$get('http://icanhazip.com')
    console.log(context)
    return res
  },
}
</script>
