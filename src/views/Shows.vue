<template>
  <div class="shows">
    <div>
      <a class="bit-widget-initializer" data-artist-name="id_15392430" data-background-color="black" data-separator-color="rgba(255,122,122,1)" data-text-color="rgba(246,246,246,1)" data-font="Helvetica" data-auto-style="true" data-display-local-dates="true" data-local-dates-position="tab" data-display-past-dates="true" data-display-details="true" data-display-lineup="false" data-display-start-time="false" data-social-share-icon="true" data-display-limit="all" data-date-format="MMM. D, YYYY" data-date-orientation="horizontal" data-date-border-color="#08C3BA" data-date-border-width="1px" data-date-border-radius="10px" data-event-ticket-cta-size="medium" data-event-ticket-text="TICKETS" data-event-ticket-icon="false" data-event-ticket-cta-text-color="#FFFFFF" data-event-ticket-cta-bg-color="rgba(255,0,4,1)" data-event-ticket-cta-border-color="rgba(255,0,4,1)" data-event-ticket-cta-border-width="0px" data-event-ticket-cta-border-radius="4px" data-sold-out-button-text-color="#FFFFFF" data-sold-out-button-background-color="#9B9B9B" data-sold-out-button-border-color="rgba(255,0,4,1)" data-sold-out-button-clickable="true" data-event-rsvp-position="left" data-event-rsvp-cta-size="medium" data-event-rsvp-text="SET REMINDER" data-event-rsvp-icon="false" data-event-rsvp-cta-text-color="rgba(255,0,4,1)" data-event-rsvp-cta-bg-color="#FFFFFF" data-event-rsvp-cta-border-color="rgba(255,0,4,1)" data-event-rsvp-cta-border-width="1px" data-event-rsvp-cta-border-radius="4px" data-follow-section-position="top" data-follow-section-alignment="center" data-follow-section-header-text="Tour Dates" data-follow-section-cta-size="small" data-follow-section-cta-text="FOLLOW" data-follow-section-cta-icon="true" data-follow-section-cta-text-color="#FFFFFF" data-follow-section-cta-bg-color="rgba(255,0,4,1)" data-follow-section-cta-border-color="rgba(255,0,4,1)" data-follow-section-cta-border-width="0px" data-follow-section-cta-border-radius="4px" data-play-my-city-position="bottom" data-play-my-city-alignment="Center" data-play-my-city-header-text="Don’t see a show near you?" data-play-my-city-cta-size="medium" data-play-my-city-cta-text="REQUEST A SHOW" data-play-my-city-cta-icon="true" data-play-my-city-cta-text-color="#FFFFFF" data-play-my-city-cta-bg-color="rgba(255,0,4,1)" data-play-my-city-cta-border-color="rgba(255,0,4,1)" data-play-my-city-cta-border-width="0px" data-play-my-city-cta-border-radius="4px" data-language="en" data-widget-width="" data-div-id="" data-app-id="" data-affil-code="undefined" data-bit-logo-position="bottomRight" data-bit-logo-color="#CCCCCC"></a>
    </div>
  </div>
</template>

<script>
export default {
  mounted() {
    let bandsInTown = document.createElement("script");
    bandsInTown.setAttribute("src", "https://widget.bandsintown.com/main.min.js");
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
