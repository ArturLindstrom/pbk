<template>
    <div class="home-container  ">
        <main-component />
    </div>
</template>

<script setup>
import MainComponent from '../components/MainComponent.vue'
</script>

<style scoped lang='scss'>

.home-container {
    display: grid;
    place-items: center;
    height: 100vh;
    width: 100%;
    background: url('/assets/p.svg'), linear-gradient(#e5d5dc, rgb(216, 174, 185));
    background-size: 4rem;
    background-color: red;
}

</style>