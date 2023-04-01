<script>
  export default {
    name: 'User',
    props: {
      name: String,
      handle: String
    }
  }
</script>

<template>
    <span class="user">
        <span class="name">{{ name }}</span>
        <span class="handle">@{{ handle }}</span>
      </span>
</template>

<style scoped>
</style>
