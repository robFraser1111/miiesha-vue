<template>
    <div id="home">
        <iframe src="https://open.spotify.com/embed/artist/1ehGGQnc7E28DNwhvnFuyL" width="300" height="420" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>

				
				<p style=""><a href="https://Miiesha-Music.lnk.to/SmokeAndMirrors" target="_blank"><img src="~@/assets/MIIESHA_Smoke+Mirrors.webp" style="width: 100%; max-width:400px;"></a><br>Smoke & Mirrors double EP <a href="https://Miiesha-Music.lnk.to/SmokeAndMirrors" target="_blank">OUT NOW</a></p>

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
		#home p {
        color: #fff;
				margin-top: 40%;
    }
		#home p a {
        color: #fff;
    }
		#home p a:hover {
        color: #fff; text-decoration: none;
    }
		#app {
            background-position: center top ;
        }

    @media only screen and (max-width: 600px) {
        #app {
            background-position: 49% 0;
        }
				#home p {
					margin-top: 140%;
				}
    }
    
</style>
