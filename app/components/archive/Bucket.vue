<template>
    <article class=" flex-1 p-6 rounded-xl" :class="className">
      <div class="font-bold text-xl">{{title}}</div>
      <div>
        <slot/>
    </div>
    </article>
</template>
<script setup>
const props = defineProps({
    title:{
        default: 'No Value'
    }, 
    body:{
        default: ''
    }, 
    className:{
        default: 'bg-red-600'
    }
})
</script>