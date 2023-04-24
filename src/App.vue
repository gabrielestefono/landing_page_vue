<template>
  <div>
    <HeaderComponent/>
    <MainComponent/>
  </div>
</template>

<script>
import HeaderComponent from './components/Header.vue';
import MainComponent from './components/Main.vue';

export default {
  name: 'Container',
  components: {
    HeaderComponent, MainComponent
  }
}
</script>

<style>
  @import url(./assets/css/reset.css);
  body{
    min-width: 100vw;
    min-height: 100vh;
    background-image: url(./assets/img/bg-mobile.svg);
    background-color: #674baf;
    font-family: 'Poppins', sans-serif;
}

@media screen and (min-width: 376px) {
    body{
        background-image: url(./assets/img/bg-desktop.svg);
        display: flex;
        flex-direction: column;
    }
}
</style>
