<template>
    <div id="home">
        <iframe src="https://open.spotify.com/embed/artist/1ehGGQnc7E28DNwhvnFuyL" width="300" height="420" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
    </div>
</template>

<script>
export default {
    name: 'Home',
}
</script>

<style>
    
    #home {
        display: flex;
        align-items: center;
        justify-content: center;
        padding: 30px;
    }

    #home iframe {
        display: none;
    }

    @media only screen and (max-width: 600px) {
        #app {
            background-position: -200px 0;
        }
    }
    
</style>
