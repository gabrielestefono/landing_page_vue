<template>
    <main class="main">
        <LeftSide/>
        <RightSide/>
    </main>
</template>

<script>
import LeftSide from './LeftSide.vue';
import RightSide from './RightSide.vue';
export default {
    name: "MainComponent",
    components: {
        LeftSide, RightSide
    }
}
</script>

<style>
@media screen and (min-width: 376px) {
    .main{
        display: flex;
        justify-content: center;
        gap: 64px;
        margin-top: 6rem;
    }
}
</style>