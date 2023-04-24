<template>
    <header class="header">
        <nav class="header__navbar">
            <img :src="image" :alt="alt" class="header__navbar--img">
        </nav>
    </header>
</template>

<script>
    import logo from "../assets/img/logo.svg";
    export default {
        name: "HeaderComponent",
        data () {
            return{
                image: logo,
                alt: "logotipo Huddle"
            }
        }
    }
</script>

<style>
.header{
    width: 100vw;
}

.header__navbar--img{
    width: 7.5rem;
    height: 19px;
    margin-left: 40px;
    margin-top: 38px;
}

@media screen and (min-width: 376px) {
    .header__navbar--img{
        width: 12.5rem;
        height: 2rem;
        margin-left: 80px;
        margin-top: 64px;
        transform: scale(1.05);
    }
}
</style>