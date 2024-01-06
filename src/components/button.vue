<script setup>
const props = defineProps(["text", "color"]);
const emits = defineEmits(['handler'])

const clickHandler = () => emits('handler');
const clickYes = () => emits ('yesButton')


</script>

<template>
  <button
    :class="{
      primary: props.color == 'primary',
      secondary: props.color == 'secondary',
    }"
    @click="clickHandler"
  >
    {{ props.text }}
  </button>
</template>

<style scoped>
button {
  border-radius: 20px;
  padding: 30px;
  margin: 0 12px;
  background-color: bisque;
  font-size: 32px;
}
.primary {
  background-color: purple;
}
.secondary {
  background-color: green;
}
</style>
