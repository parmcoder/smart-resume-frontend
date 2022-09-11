<script setup lang="ts">
import { defineComponent } from 'vue';

defineProps<{
    text: string,
    url: string
}>()
</script>

<template>
    <div>
        <a :href="url" target="_blank" class="container"> <i>
                <slot name="icon"></slot>
            </i>
            <h1 style="margin-left: 20px">
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
</style>

<script lang="ts">
export default defineComponent(
    {
        data() {
            return {
                count: 1
            }
        }
    })
</script>