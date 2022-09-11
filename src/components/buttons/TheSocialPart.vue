<script setup lang="ts">
import SocialButton from "./SocialButton.vue";
import IconCommunity from "../icons/IconCommunity.vue";
</script>

<template>
    <div class="container">
        <SocialButton text="GITHUB" url="https://www.github.com/parmcoder">
            <template #icon>
                <IconCommunity></IconCommunity>
            </template>
        </SocialButton>
        <SocialButton text="LinkedIn" url="https://www.linkedin.com/in/parmcoder">
            <template #icon>
                <IconCommunity></IconCommunity>
            </template>
        </SocialButton>
    </div>
</template>

<style scoped>
.container {
    display: flex;
    flex-direction: row;
    justify-content: center;
    min-width: 500px;
}
</style>