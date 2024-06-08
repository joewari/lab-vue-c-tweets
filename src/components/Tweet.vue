<template>
  <div class="tweet">
    <ProfileImg :childImage="Image" />

    <div class="body">
      <div class="top">
        <span class="user">
          <User :nameChild="Name" />
          <User :handleChild="Handle" />
        </span>

        <Time :timeStampChild="TimeStamp" />
      </div>

      <Message :childMessage="message" />

      <Action />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<style scoped>
a {
  color: #42b983;
}
</style>
<script setup>
import Message from "./Message.vue";
import User from "./User.vue";
import Time from "./Timestamp.vue";
import ProfileImg from "./ProfileImage.vue";
import Action from "./Actions.vue";
defineProps({
  Name: {
    type: String,
  },
  Image: { type: String },
  Handle: { type: String },
  TimeStamp: { type: String },
  message: { type: String },
});
</script>
