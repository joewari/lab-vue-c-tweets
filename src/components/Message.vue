<template>
  <p class="message">{{ msg }}</p>
</template>

<script setup>
import { ref, reactive, computed } from "vue";
defineProps({
  msg: {
    type: String,
  },
});
</script>

<style scoped></style>
