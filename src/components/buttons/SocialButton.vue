<script setup lang="ts">
import { computed, useSlots } from 'vue';

defineProps<{
    text: string,
    url: string
}>()

const slots = useSlots()

const hasIconSlot = computed(() => slots.icon)
</script>

<template>
    <div>
        <a :href="url" target="_blank" :class="{ container: hasIconSlot, yat: !hasIconSlot }">
            <i v-if="hasIconSlot">
                <slot name="icon"></slot>
            </i>
            <h1 :class="{ left: hasIconSlot }">
                {{text}}
            </h1>

        </a>
    </div>
</template>

<style scoped>
.yat {
    display: flex;
    width: 250px;
    height: 75px;
    align-items: center;
    justify-content: center;
}

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

@media (max-width: 1024px) {
    .container {
        justify-content: start;
    }

    i {
        margin-left: 50px;
    }
}
</style>