<template>
  <div>
    <HeaderComponent/>
    <MainComponent/>
    <FooterComponent/>
  </div>
</template>

<script>
import HeaderComponent from './components/Header.vue';
import MainComponent from './components/Main.vue';
import FooterComponent from './components/Footer.vue';

export default {
  name: 'Container',
  components: {
    HeaderComponent, MainComponent, FooterComponent
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
