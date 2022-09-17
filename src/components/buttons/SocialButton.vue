<script setup lang="ts">
defineProps<{
    text: string,
    url: string
}>()
</script>

<template>
    <div>
        <a :href="url" target="_blank" class="container">
            <i>
                <slot name="icon"></slot>
            </i>
            <h1 :class="{ left: this.$slots.icon }">
                {{text}}
            </h1>

        </a>
    </div>
</template>

<style scoped>
.container {
    display: flex;
    width: 250px;
    height: 75px;
    justify-content: center;
    align-items: center;

}

.left {
    margin-left: 20px;
}
</style>