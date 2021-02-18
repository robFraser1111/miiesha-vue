<template>
  <div id="app" :style="{ backgroundImage: `url('${background}')` }">
    <div class="menu">
        <a href="/">
            <img class="logo" src="~@/assets/miiesha-logo-01.png" alt="Miiesha">
        </a>
        <ul>
            <router-link to="/bio">
                <li>BIO</li>
            </router-link>
            <router-link to="/watch">
                <li>WATCH</li>
            </router-link>
            <router-link to="/contact">
                <li>CONTACT</li>
            </router-link>
        </ul>
    </div>

    <transition name="slide" mode="out-in">
      <router-view :key="$route.path" />
    </transition>

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
        <p>
          <small>
          Photography by <a href="https://www.instagram.com/clarenicaa/" target="_blank">Clare Nica</a> and <a href="https://www.instagram.com/thommitchell/" target="_blank">Thom Mitchell</a>
          <br>
          Website powered by <a href="https://roo.digital" target="_blank">RooDigital</a>
          </small>
        </p>
    </div>
  </div>
</template>

<script>
// Import background images
import homeBackground from '@/assets/miiesha-01.jpg'
import bioBackground from '@/assets/miiesha-02.jpg'
import watchBackground from '@/assets/miiesha-03.jpg'
import contactBackground from '@/assets/miiesha-04.jpg'

// Data store
export default {
    data() {
      return {
        background: homeBackground,
      }
    },

  // watch function to dynamically change background image for #app
  watch: {
    '$route' () {
      if (this.$route.path === '/') {
        this. background = homeBackground
      }
      else if (this.$route.path === '/bio') {
        this. background = bioBackground
      }  
      else if (this.$route.path === '/watch') {
        this. background = watchBackground
      }  
      else if (this.$route.path === '/contact') {
        this. background = contactBackground
      }  
      else {
        this. background = homeBackground
      }
    }
  }
}
</script>

<style scoped>
  .menu a {
        text-decoration: none!important;
    }
</style>

<style>

@font-face {
  font-family: "Varela Round";
  src: local("Varela Round"),   url(./assets/VarelaRound-Regular.ttf) format("truetype");
  }


#app {
  font-family: "Varela Round", Roboto, Arial;
  background-color: rgb(0, 0, 0, 0.5);
  background-position: center;
  background-size: cover;
  background-blend-mode: color;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 0;
  max-width: 2560px;
  display: grid;
  grid-template-rows: auto 1fr auto;
  min-height: 100vh;
}

body {
  margin: 0;
}

.logo {
  display: block;
  margin: 0 auto;
  padding: 20px;
  width: 240px;
  height: auto;
}

ul {
  list-style: none;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0;
  padding: 0;
}
  
.menu li {
  padding: 10px 20px;
  font-size: 18px;
  font-weight: 400;
  text-align: center;
  color: #ffffff;
  transition: ease-in-out;
  transition-duration: .2s;
}

p, h1, h2, h3, h4, h5, h6 {
  line-height: normal;
}

p {
  font-size: 1.2rem;
  line-height: 1.7rem;
  font-weight: 300;
}

#footer, #footer a {
  color: #ffffff;
}

#footer p {
  font-size: 16px;
}

.social-icons li {
  padding: 10px 20px;
  transition: ease-in-out;
  transition-duration: .2s;
}

li:hover {
    opacity: 0.75;
}

.slide-enter-active,
.slide-leave-active {
  transition: opacity .2s, transform .2s;
}

.slide-enter,
.slide-leave-to {
  opacity: 0;
  animation: fadeIn .2s ease-in;
}

</style>
