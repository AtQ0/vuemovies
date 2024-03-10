<template>
    <div class="navbar">
        <div class="hamburger-and-links-container">
            <div class="hamburger-container">

            </div>

        </div>

        <h1 class="page-logo"><span class="vue-part-of-logo">Vue</span>Movies</h1>
    </div>

</template>

<script setup>

</script>

<style scoped>

.navbar{
    width: 100vw;
    padding-top: 5px;
    padding-bottom: 5px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: fixed;
    top: 0px;
    z-index: 2;
    background-color: rgba(0, 0, 0, 0.5);
    backdrop-filter: blur(2px);
}

.page-logo{
    width: fit-content;
    background-color: green;
}

.vue-part-of-logo{
    color: var(--vue-green);
}


</style>
