<template>
    <footer class="footer">
        <div class="footer__link" id="facebook"></div>
        <div class="footer__link" id="twitter"></div>
        <div class="footer__link" id="instagram"></div>
    </footer>
</template>

<script>
export default {
    name: "FooterComponent"
}
</script>

<style>
.footer{
    width: calc((28px * 3) + 22px);
    margin: 0 auto;
    margin-top: 4rem;
    justify-content: space-between;
    display: flex;
}

.footer__link{
    width: 28px;
    height: 28px;
    margin-bottom: 2.5rem;
}

#facebook{
    background-image: url(../assets/img/facebook.svg);
}

#twitter{
    background-image: url(../assets/img/twitter.svg);
}

#instagram{
    background-image: url(../assets/img/instagram.svg);
}

@media screen and (min-width: 376px) {
    .footer{
        width: auto;
        flex: 1;
        right: 4rem;
        align-items: flex-end;
        justify-content: flex-end;
        position: absolute;
        bottom: 2rem;
    }

    .footer__link{
        width: 40px;
        height: 40px;
        margin-right: 1rem;
        background-repeat: no-repeat;
        background-size: cover;
        cursor: pointer;
    }

    #facebook:hover{
        background-image: url(../assets/img/facebook_hover.svg);
        transition: 200ms;
    }
    
    #twitter:hover{
        background-image: url(../assets/img/twitter_hover.svg);
        transition: 200ms;
    }
    
    #instagram:hover{
        background-image: url(../assets/img/instagram_hover.svg);
        transition: 200ms;
    }
    
}
</style>