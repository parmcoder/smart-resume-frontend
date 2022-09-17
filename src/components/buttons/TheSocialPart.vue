<script setup lang="ts">
import SocialButton from "./SocialButton.vue";
import IconOnlyfan from "../icons/IconOnlyfan.vue";
</script>

<template>
    <div class="container">
        <SocialButton text="GITHUB" url="https://www.github.com/parmcoder">
            <template #icon>
                <font-awesome-icon icon="fa-brands fa-github" class="fa-xl"/>
            </template>
        </SocialButton>
        <SocialButton text="LinkedIn" url="https://www.linkedin.com/in/parmcoder">
            <template #icon>
                <font-awesome-icon icon="fa-brands fa-linkedin" class="fa-xl"/>
            </template>
        </SocialButton>
        <SocialButton text="OnlyFans" url="https://bit.ly/3BlS71b">
            <template #icon>
                <IconOnlyfan></IconOnlyfan>
            </template>
        </SocialButton>
        <SocialButton text="Twitch" url="https://www.twitch.tv/lenmalendi">
            <template #icon>
                <font-awesome-icon icon="fa-brands fa-twitch" class="fa-xl"/>
            </template>
        </SocialButton>
    </div>
    <div class="container">
        <SocialButton text="Instagram" url="https://www.github.com/parmcoder">
            <template #icon>
                <font-awesome-icon icon="fa-brands fa-instagram" class="fa-xl"/>
            </template>
        </SocialButton>
        <SocialButton text="Discord" url="https://www.linkedin.com/in/parmcoder">
            <template #icon>
                <font-awesome-icon icon="fa-brands fa-discord" class="fa-xl"/>
            </template>
        </SocialButton>
        <SocialButton text="🎮😈💻" url="https://y.at/%F0%9F%8E%AE%F0%9F%98%88%F0%9F%92%BB">
        </SocialButton>
    </div>
</template>

<style scoped>
.container {
    display: flex;
    flex-direction: row;
    justify-content: center;
    /* min-width: 500px; */
}
@media (max-width: 1024px) {
    .container {
        flex-direction: column;
        align-items: center;
    }
}
</style>