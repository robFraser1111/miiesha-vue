<template>
    <div class="shows">
        <div>
            <a
                class="bit-widget-initializer"
                data-artist-name="id_15392430"
                data-font="Helvetica"
                data-language="en"
                data-display-details="false"
                data-text-color="#000000"
                data-background-color="#ffffff"
                data-separator-color="#DDDDDD"
                data-popup-background-color="#ffffff"
                data-link-color="#A2A2A2"
                data-link-text-color="#FFFFFF"
            ></a>
        </div>
    </div>
</template>

<script>
export default {
    mounted() {
        let bandsInTown = document.createElement("script");
        bandsInTown.setAttribute(
            "src",
            "https://widget.bandsintown.com/main.min.js"
        );
        document.head.appendChild(bandsInTown);
    },
    name: "Shows",
};
</script>

<style>
.shows {
    margin-top: 60px;
    margin-bottom: 60px;
    max-width: 1200px;
    display: flex;
    justify-self: center;
    
}

@media only screen and (max-width: 600px) {
    #app {
        background-position: 600px 0;
    }
    .bit-event {
        flex-direction: column !important;
    }
    .shows,
    .bit-widget-container {
        max-width: 375px;
    }
}
</style>
