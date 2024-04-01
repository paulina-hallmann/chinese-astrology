<template>
    <PageHeader></PageHeader>
    <ZodiacHeader></ZodiacHeader>
    zodiac sign page content
    <h1>{{ route.params.zodiacSign }}</h1>
</template>

<script setup lang="ts">

const route = useRoute()

</script>