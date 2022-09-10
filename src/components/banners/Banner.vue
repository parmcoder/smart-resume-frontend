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

<style lang="scss">
.banner {
    color: white;
    min-width: 500px;
    min-height: 200px;
}
</style>