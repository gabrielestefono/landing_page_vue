<template>
    <main class="main">
        <LeftSide/>
    </main>
</template>

<script>
import LeftSide from './LeftSide.vue';
//import RightSide from './RightSide.vue';
export default {
    name: "MainComponent",
    components: {
        LeftSide, //RightSide
    }
}
</script>

<style>
.main{
    display: flex;
    justify-content: center;
    gap: 64px;
    margin-top: 6rem;
}
</style>