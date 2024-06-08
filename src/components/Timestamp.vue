<template>
  <span class="timestamp">{{ timeStampChild }}</span>
</template>

<script setup>
import { ref, reactive, computed } from "vue";
defineProps({
  timeStampChild: {
    type: String,
  },
});
</script>

<style scoped></style>
