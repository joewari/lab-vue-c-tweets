<template>
  <img :src="childImage" class="profile" alt="profile" />
</template>

<script setup>
import { ref, reactive, computed } from "vue";
defineProps({
  childImage: {
    type: String,
  },
});
</script>

<style scoped></style>
