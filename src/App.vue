<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
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

    .main{
        display: flex;
        justify-content: center;
        gap: 64px;
        margin-top: 6rem;
    }
}
</style>
