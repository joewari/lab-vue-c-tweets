<template>
  <span class="timestamp">{{ timeStamp }}</span>
</template>

<script setup>
import { ref, reactive, computed } from "vue";
defineProps({
  timeStamp: {
    type: String,
  },
});
</script>

<style scoped></style>
