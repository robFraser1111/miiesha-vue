<script>
export default {
  mounted() {
    // Mail Chimp scripts
    let mailChimpStyles = document.createElement("link");
    mailChimpStyles.setAttribute("href", "https://cdn-images.mailchimp.com/embedcode/classic-10_7_dtp.css");
    document.head.appendChild(mailChimpStyles);
    // Mail Chimp styles
    let mailChimpScript = document.createElement("script");
    mailChimpScript.setAttribute("src", "https://s3.amazonaws.com/downloads.mailchimp.com/js/mc-validate.js");
    document.head.appendChild(mailChimpScript);
  },
  name: "Shows",
};

// (function($) {
//   window.fnames = new Array();
//   window.ftypes = new Array();
//   fnames[0] = "EMAIL";
//   ftypes[0] = "email";
//   fnames[1] = "FNAME";
//   ftypes[1] = "text";
//   fnames[2] = "LNAME";
//   ftypes[2] = "text";
//   fnames[3] = "ADDRESS";
//   ftypes[3] = "address";
//   fnames[4] = "PHONE";
//   ftypes[4] = "phone";
//   fnames[5] = "BIRTHDAY";
//   ftypes[5] = "birthday";
// })(jQuery);
// var $mcj = jQuery.noConflict(true);
</script>

<style scoped>
#mc_embed_signup {
  background: none;
  width: 100%;
}

.response, .mce_inline_error {
  margin-top: 10px;
}

h2 {
  margin: 0;
}

form {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 20px;
  background: rgb(0, 13, 19, 0.5);
  color: #fff;
}

input {
  width: 180px;
  padding: 5px;
  margin-bottom: 5px;
}

button {
  background: #2c3e50;
  color: #fff;
  border: none;
  padding: 10px;
  border-radius: 5px;
  font-size: 16px;
  cursor: pointer;
  margin-top: 5px;
  width: 192px;
}
</style>

<template>
  <div>
    <form action="https://miiesha.us12.list-manage.com/subscribe/post?u=8d1035d26e1dc1e203204657f&amp;id=770e85a280" method="post" id="mc-embedded-subscribe-form" name="mc-embedded-subscribe-form" class="validate" target="_blank" novalidate>
      <div id="mc_embed_signup_scroll">
        <div class="mc-field-group">
          <input type="email" value="" placeholder="Email" name="EMAIL" class="required email" id="mce-EMAIL" />
        </div>
        <div id="mce-responses" class="clear foot">
          <div class="response" id="mce-error-response" style="display:none"></div>
          <div class="response" id="mce-success-response" style="display:none"></div>
        </div>
        <!-- real people should not fill this in and expect good things - do not remove this or risk form bot signups-->
        <div style="position: absolute; left: -5000px;" aria-hidden="true"><input type="text" name="b_8d1035d26e1dc1e203204657f_770e85a280" tabindex="-1" value="" /></div>
      </div>
      <button type="submit">Subscribe</button>
    </form>
  </div>
</template>
