<template>
  <p class="message">{{ childMessage }}</p>
</template>

<script setup>
import { ref, reactive, computed } from "vue";
defineProps({
  childMessage: {
    type: String,
  },
});
</script>

<style scoped></style>
