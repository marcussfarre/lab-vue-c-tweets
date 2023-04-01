<script>
  export default {
    props: {
      image: String
    },
  }
</script>

<template>
    <img
      :src="image"
      class="profile"
      alt="profile"
    />
</template>

<style scoped>
</style>
