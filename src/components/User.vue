<template>
  <span class="user">
    <span class="name">{{ nameChild }}</span>
    <span class="handle">{{ handleChild }}</span>
  </span>
</template>

<script setup>
import { ref, reactive, computed } from "vue";
defineProps({
  nameChild: {
    type: String,
  },
  handleChild: {
    type: String,
  },
});
</script>

<style scoped></style>
