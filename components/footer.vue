<template>
  <section>
    <v-footer height="100%" class="hidden-xs-and-down my-footer black--text">
      <v-layout row wrap>
        <v-flex sm4 xs12 px-5 text-sm-left class="white">
          <nuxt-link to="/"><img src="/assets/logo.png" class="myLogo" /></nuxt-link><br/>
          <div class="mt-3 body-2">ABOUT US</div>
          <div class="mt-3 pr-4">Moneybag.ng empowers people to build and manage their financial future by creating a transparent avenue to save.</div>

          <table width="135" border="0" cellpadding="2" cellspacing="0" title="Click to Verify - This site chose GeoTrust SSL for secure e-commerce and confidential communications.">
          <tr>
          <td width="135" align="center" valign="top"><script type="text/javascript" src="https://seal.geotrust.com/getgeotrustsslseal?host_name=moneybag.ng&amp;size=M&amp;lang=en"></script><br />
          <a href="http://www.geotrust.com/ssl/" target="_blank"  style="color:#000000; text-decoration:none; font:bold 7px verdana,sans-serif; letter-spacing:.5px; text-align:center; margin:0px; padding:0px;"></a></td>
          </tr>
          </table>
        </v-flex>
        
        <v-flex class="second-section" sm8>
          <v-layout row wrap  px-5 mb-5>
            <v-flex sm4>
              <div class="mb-4 body-2">QUICK LINKS</div>
              <nuxt-link to="/about"><div>About Us</div></nuxt-link>
              <nuxt-link to="/faq2"><div>FAQs</div></nuxt-link>
              <nuxt-link to="/about#how"><div>How it Works</div></nuxt-link>
              <nuxt-link to="/terms"><div>Terms of Use</div></nuxt-link>
              <a href="mailto:support@nuture.tech" target="_top">Email Us</a>
            </v-flex>

            <v-flex sm4 pr-4>
              <div class="mb-4 body-2">CONTACT INFO</div> 
              <div>1B, Adeniji street, Adeniji Estate, off Wemco road, Ikeja, Lagos.</div>
              <div class="mt-3"><a href="tel:070066639224">0700MONEYBAG</a></div>
              <a href="mailto:support@nuture.tech" target="_top" class="">support@nuture.tech</a>
            </v-flex>

            <v-flex sm4>
              <div class="mb-4 body-2">GET SOCIAL WITH US</div> 
              <div>Connect with us on any of our Social Media accounts.</div>
              <div class="mt-4">
              <a target="_blank" href="https://www.facebook.com/moneybagng/"><img src="/assets/facebook.png" alt="" class="mr-3"></a>
              <a target="_blank" href="https://www.instagram.com/moneybagng/"><img src="/assets/instagram.png" alt="" class="mr-3"></a>
              <a target="_blank" href="https://twitter.com/moneybagng"><img src="/assets/twitter.png" alt="" class=""></a>
            </div>
            </v-flex>
          </v-layout>

          <v-divider></v-divider>
          <v-layout pl-5 py-3 justify-space-between class="footer-bottom">
            <div>2018 Copyright. All Rights Reserved</div>
            <nuxt-link to="/privacy"><div>Privacy Policy</div></nuxt-link>
          </v-layout>
        </v-flex>
      </v-layout>
    </v-footer>

    <v-footer height="100%" class="mygrey white--text footer-mobile-wrapper">
      <div class="footer-padding">
        <v-layout row wrap>
          <v-flex xs6>
            <div class="mb-1 body-2">QUICK LINKS</div>
            <nuxt-link class="white--text" to="/about"><div>About Us</div></nuxt-link>
            <nuxt-link class="white--text" to="/faq2"><div>FAQs</div></nuxt-link>
            <!-- <nuxt-link class="white--text" to="/about#how"><div>How it Works</div></nuxt-link> -->
            <nuxt-link class="white--text" to="/terms"><div>Terms of Use</div></nuxt-link>
            <nuxt-link class="white--text" to="/privacy"><div>Privacy Policy</div></nuxt-link>
            <a href="mailto:support@nuture.tech" target="_top" class="white--text">Email Us</a>
          </v-flex>
          <v-flex xs6>
            <div class="mb-1 body-2">CONTACT INFO</div>
            <div>1B, Adeniji street, Adeniji Estate, off Wemco road, Ikeja, Lagos.</div>
            <div class="mt-2"><a class="white--text" href="tel:070066639224">0700MONEYBAG</a></div>
            <a href="mailto:support@nuture.tech" target="_top" class="white--text">support@nuture.tech</a>
          </v-flex>
        </v-layout>

        <v-flex class="center mt-4">
          <div class="mb-1 body-2">GET SOCIAL WITH US</div> 
          <div>Connect with us on any of our Social Media accounts.</div>
          <div class="mt-3">
            <a target="_blank" href="https://www.facebook.com/moneybagng/"><img src="/assets/facebook.png" alt="" class="mr-3"></a>
            <a target="_blank" href="https://www.instagram.com/moneybagng/"><img src="/assets/instagram.png" alt="" class="mr-3"></a>
            <a target="_blank" href="https://twitter.com/moneybagng"><img src="/assets/twitter.png" alt="" class=""></a>
          </div>
        </v-flex>
      </div>

      <table width="135" border="0" cellpadding="2" cellspacing="0" title="Click to Verify - This site chose GeoTrust SSL for secure e-commerce and confidential communications.">
      <tr>
      <td width="135" align="center" valign="top"><script type="text/javascript" src="https://seal.geotrust.com/getgeotrustsslseal?host_name=moneybag.ng&amp;size=M&amp;lang=en"></script><br />
      <a href="http://www.geotrust.com/ssl/" target="_blank"  style="color:#000000; text-decoration:none; font:bold 7px verdana,sans-serif; letter-spacing:.5px; text-align:center; margin:0px; padding:0px;"></a></td>
      </tr>
      </table>

      <v-flex class="center mt-4 py-2 black">
        <div>2018 Copyright. All Rights Reserved</div>
      </v-flex>
    </v-footer>
  </section>
</template>

<style lang="scss" scoped>
.my-footer {
  padding-top: unset !important;  

  @media only screen and (max-width: 760px) {
    display: none !important;
  }
}

.footer-bottom {
  padding-right: 10%;
}

a {
  text-decoration: none;
  color: black;
}

.myLogo {
  width: 200px;
  margin-top: 15%;
  margin-bottom: 5%;
}

.line {
  height: 4%;
}

.second-section {
  background-color: #e9e5e5;
  padding-top: 5%;
}

.footer-mobile-wrapper {
  display: block;
  padding: 10% 0 0 0;
  font-size: 0.8em;

  @media only screen and (min-width: 760px) {
    display: none !important;
  }
}

.center {
  text-align: center;
  text-justify: center;
}

.footer-padding {
  padding: 0 5%;
}
</style>

