<script setup lang="ts">
defineEmits({
  submit() {
    return false
  },
})
</script>

<template>
  <button @click="$emit('submit')">Comp Button</button>
</template>
