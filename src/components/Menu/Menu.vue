<script setup>
    import MenuItem from "@/components/Menu/MenuItem.vue"

    const menuFirstTitle = "Ana Sayfa 2";
    const menuSecondTitle = "İleteşim 2";

</script>

<template>
      <nav>
            <MenuItem :name="menuFirstTitle" emoji="🦄 "></MenuItem>
            <MenuItem :name="menuSecondTitle"></MenuItem>
            <MenuItem name="Yardım"></MenuItem>
           
        </nav>
</template>