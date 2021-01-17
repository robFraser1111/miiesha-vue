<template>
    <div id="footer">
        <ul class="social-icons">
            <a href="https://open.spotify.com/artist/1ehGGQnc7E28DNwhvnFuyL">
                <li><img src="~@/assets/spotify.svg" alt="Spotify"></li>
            </a>
            <a href="https://www.youtube.com/c/miiesha">
                <li><img src="~@/assets/youtube.svg" alt="YouTube"></li>
            </a>
            <a href="https://www.facebook.com/Miiesha/">
                <li><img src="~@/assets/facebook.svg" alt="Facebook"></li>
            </a>
            <a href="https://www.instagram.com/miieshaofficial/">
                <li><img src="~@/assets/instagram.svg" alt="Instagram"></li>
            </a>
            <a href="https://twitter.com/miieshaofficial">
                <li><img src="~@/assets/twitter.svg" alt="Twitter"></li>
            </a>
        </ul>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
    ul {
        list-style: none;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    
    li {
        padding: 20px;
        color: #ffffff;
        transition: ease-in-out;
        transition-duration: .2s;
    }

    li:hover {
        opacity: 0.75;
    }
</style>