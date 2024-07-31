<script setup>
    defineProps({
        services: Array 
    });

</script>

<template>
    <div v-for="service of services" :key="service.name" class="service__item-wrapper">
        <img class="service__item-image" :src="service.imagePath" alt="">
        <h3 class="service__item-h3">{{ service.name }}</h3>
        <p class="service__item-description">
            {{ service.description }}
        </p>
    </div>
    
</template>