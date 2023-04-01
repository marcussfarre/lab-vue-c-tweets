<script>
  export default {
    name: 'Message',
    props: {
      message: String
    },
  }
</script>

<template>
    <p class="message">
        {{ message }} 🚀
    </p>
</template>

<style scoped>
</style>
