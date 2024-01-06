<script setup>
const props = defineProps(['name','lastName', 'emoji','age'])
</script>

<template>
    <li v-if="props.age > 10" style="color: red;">
     {{ props.name }} {{ props.lastName }} {{ props.emoji }} {{ props.age }}
    </li>

    <li v-else>
        {{ props.name }}
    </li>
</template>