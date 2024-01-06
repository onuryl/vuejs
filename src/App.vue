<script setup>
import PopupComponent from "@/components/popup.vue";
import SubscribeComponent from "@/components/subscribe.vue";
import ButtonComponent from "@/components/button.vue"
import ListingComponent from "@/components/listin.vue"

const parentHandler = () => console.log('Parrrent Handlerr')
const yesbutonu = () => console.log('yes butonuna basildi')

const subtitle = "Limited Time Offer🦄"
const popimage ="https://images.unsplash.com/photo-1513104890138-7c749659a591?q=100&w=160&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"

</script>

<template>

<ListingComponent></ListingComponent>
<br>
<hr>
<br>

<ButtonComponent text="Bu Buton rengi Farklı" color="primary" @handler="parentHandler"></ButtonComponent>
<PopupComponent :subtitle="subtitle" text="Register and get 25% off on your next order" :image="popimage">
<template #bottom><SubscribeComponent></SubscribeComponent></template>

</PopupComponent>

<PopupComponent subtitle="Yeni Bir popop" text="Beğendik miiii???" :image="popimage">
<template #bottom>
  <ButtonComponent text="Evet" color="secondary" @handler="yesbutonu"></ButtonComponent>
  <ButtonComponent text="Hayır"></ButtonComponent>
</template>

</PopupComponent>

</template>


