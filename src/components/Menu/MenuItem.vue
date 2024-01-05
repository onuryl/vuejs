<script setup>
const props = defineProps (["name","emoji"])

</script>

<template>
    <a href="#">
        <span>{{ props.emoji}}</span>
              {{ props.name }}
    </a>
</template>

<style scoped>
a {
    padding:  8 20px;
    margin: 0 20px;
    background-color: blueviolet;
}


</style>