<script setup>
const props = defineProps (["subtitle", "text","image"])


</script>


<template>
    <div class="popup">
        <div class="popup_image">
            <img :src="props.image"
                alt="pizza">
        </div>
        <div class="popup_content">
            <h3>{{props.subtitle}}</h3>
            <p>{{props.text}}</p>
           <slot name="bottom"></slot>
        </div>
    </div>
</template>

<style scoped>

.popup {
  display: flex;
  flex-direction: row;
  align-items: flex-start;
  justify-content: flex-start;
  margin: 20px ;
  width: 480px;
  max-width: 480px;
  background-color: black;
  border-radius: 20px;
  padding: 20px;
  color: white;
}
.popup_image {
  width: 160px;
  max-width: 160px;
  background-color: aqua;
}

.popup_content h3 {
    font-size: 18px;
  }
  .popup_content p {
    font-size: 48px;
  }

  .popup_subscribe {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
  }
</style>