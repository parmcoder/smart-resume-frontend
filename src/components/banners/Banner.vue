<script setup lang="ts">
defineProps<{
  msg: string
}>()
</script>

<template>
    <div class="banner">
        {{ msg }}
    </div>
</template>

<style scoped>
.banner {
    color: var(--color-text);
    background-color: var(--color-background-soft);
    height: 200px;

    font-size: 100px;
    display: flex;
    align-items: center;
    justify-content: center;
}

@media (max-width: 1024px) {
    .banner{
        font-size: 50px;
    }
}
</style>