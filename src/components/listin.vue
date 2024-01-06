<script setup>
import Listenitem from '@/components/listinitem.vue'

const data = [
{
    id: 1,
    name: 'Onur',
    lastName: 'Yilmaz',
    emoji:'😿',
    age: '33'
},
{
    id: 2,
    name:'Tugba',
    lastName:'Yalcin',
    emoji:'🦄',
    age:'30'
},
{
    id: 3,
    name:'Kerem',
    lastName:'Altun',
    emoji:'🥸',
    age:'25'
}
]

</script>


<template>
<div>
    <ul>
        <Listenitem v-for="person in data" :key='person.id'
           :age="person.age" :name="person.name" :lastName="person.lastName" :emoji="person.emoji">
        </Listenitem>
    </ul>
 
</div>
</template>

