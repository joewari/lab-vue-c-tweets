<template>
  <img :src="image" class="profile" alt="profile" />
</template>

<script setup>
import { ref, reactive, computed } from "vue";
defineProps({
  image: {
    type: String,
  },
});
</script>

<style scoped></style>
