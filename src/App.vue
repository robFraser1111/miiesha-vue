<template>
  <div id="app">
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
          Photography by <a href="/" target="_blank">Clare Nica</a> and <a href="/" target="_blank">Thom Mitchell</a>
          <br>
          Website powered by <a href="https://roo.digital" target="_blank">RooDigital</a>
          </small>
        </p>
    </div>
  </div>
</template>

<style scoped>
  .menu a {
        text-decoration: none!important;
    }
</style>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
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
      padding: 20px 20px;
      font-size: 22px;
      font-weight: 400;
      text-align: center;
      color: #ffffff;
      transition: ease-in-out;
      transition-duration: .2s;
    }

    #footer, #footer a {
      color: #ffffff
    }

    .social-icons li {
      padding: 20px;
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
