<template>
  <div>
    <p>index page</p>
    <p>user with id: {{ $route.params.id }}</p>
  </div>
</template>

<script>
export default {
  validate(data) {
    return data.params.id === '1'
  },
  data() {
    return {}
  },
}
</script>
