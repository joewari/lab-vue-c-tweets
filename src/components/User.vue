<template>
  <span class="user">
    <span class="name">{{ userdata.name }}</span>
    <span class="handle">{{ userdata.handle }}</span>
  </span>
</template>

<script setup>
import { ref, reactive, computed } from "vue";

defineProps({
  userdata: Object,
});
</script>

<style scoped></style>
