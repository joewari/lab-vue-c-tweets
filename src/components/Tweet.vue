<template>
  <div class="tweet">
    <ProfileImg :image="image" />

    <div class="body">
      <div class="top">
        <span class="user">
          <User :userdata="user" />
        </span>

        <Time :timeStamp="time" />
      </div>

      <Message :msg="message" />

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
  user: {
    type: Object,
  },
  image: { type: String },
  time: { type: String },
  message: { type: String },
});
</script>
