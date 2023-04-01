<script>
  import ProfileImage from './ProfileImage.vue'
  import Actions from './Actions.vue';
  import Message from './Message.vue';
  import Timestamp from './Timestamp.vue';
  import User from './User.vue';

  export default {
      name: 'Tweet',
      props: {
        tweet: {
          user: Object,
          message: String,
          timestamp: String,
        }
      },
      components: { ProfileImage, Message, Actions, Timestamp, User }
  }
</script>

<template>
  <div class="tweet">
    <ProfileImage :image="this.tweet.user.image"/>

    <div class="body">
      <div class="top">
        <User :handle="this.tweet.user.handle" :name="this.tweet.user.name"/>
        <Timestamp :timestamp="this.tweet.timestamp"/>
      </div>
      <Message :message="this.tweet.message" />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<style scoped>
a {
  color: #42b983;
}
</style>
