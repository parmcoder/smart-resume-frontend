<template>
    <div class="frame">
        <div class="background">
            <img class="profile-pic" src="../../assets/me7.jpg" placeholder="parm's image" />

            <span class="about-info">
                My name is Parm.
            </span>
        </div>


    </div>
</template>

<style scoped>
.about-info {
    /* min-width: 200px; */
    flex: 1 0 auto;
    margin-left: 30px;
    display: flex;
    align-items: center;
    justify-content: center;
}

.profile-pic {
    width: 280px;
    height: 280px;
    top: -15px;
    left: 30px;
    border-radius: 50%;
}

.frame {
    height: 300px
}

.background {
    height: 250px;
    margin-top: 30px;
    background-color: var(--color-background-soft);
    display: flex;
}

@media screen {
    
}

</style>