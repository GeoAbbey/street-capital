<template>
  <v-app light>
    <v-navigation-drawer v-model='sideNav.model' disable-resize-watcher width='170' app overflow left persistent>
      <v-list>
        <nuxt-link to="#">
          <v-list-tile class="profile-image layout justify-center">
            <v-avatar class="profile-image-holder" size="80px">
              <img src="/ismail.jpeg" alt="">
            </v-avatar>
          </v-list-tile>
        </nuxt-link>
        <v-list-tile class="mb-3 layout justify-center">
          <nuxt-link to="/profile">
            <v-list-tile-content>
              <h3 class="body-2 black--text">Olasunkanmi Ismail</h3>
              <div class="caption grey--text"><strong>REG NO: SCE/2016/027</strong></div>
            </v-list-tile-content>
          </nuxt-link>
        </v-list-tile>
        <v-list-tile>
          <v-list-tile-action>
            <nuxt-link class="black--text" to='#'>
              <v-icon class="black--text">dashboard</v-icon>
            </nuxt-link>
          </v-list-tile-action>
          <v-list-tile-content>
            <nuxt-link class="black--text" to='#'>Home</nuxt-link>
          </v-list-tile-content>
        </v-list-tile>
        <v-list-tile>
          <v-list-tile-action>
            <nuxt-link class="black--text" to='#'>
              <v-icon class="black--text">info</v-icon>
            </nuxt-link>
          </v-list-tile-action>
          <v-list-tile-content>
            <nuxt-link class="black--text" to='#'>About</nuxt-link>
          </v-list-tile-content>
        </v-list-tile>
        <v-list-tile>
          <v-list-tile-action>
            <nuxt-link to='#'>
              <v-icon class="black--text">class</v-icon>
            </nuxt-link>
          </v-list-tile-action>
          <v-list-tile-content>
            <nuxt-link class="black--text" to='#'>Learning</nuxt-link>
          </v-list-tile-content>
        </v-list-tile>
        <v-list-tile>
          <v-list-tile-action>
            <nuxt-link to='#'>
              <v-icon class="black--text">bar_chart</v-icon>
            </nuxt-link>
          </v-list-tile-action>
          <v-list-tile-content>
            <nuxt-link class="black--text" to='#'>Challenge</nuxt-link>
          </v-list-tile-content>
        </v-list-tile>
        <v-list-tile>
          <v-list-tile-action>
            <nuxt-link to='/'>
              <v-icon class="black--text">settings_power</v-icon>
            </nuxt-link>
          </v-list-tile-action>
          <v-list-tile-content>
            <nuxt-link class="black--text" to='/'>Log Out</nuxt-link>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>

    <v-toolbar absolute flat height="100px" color="transparent" dark>
      <v-toolbar-side-icon dark @click.stop='sideNav.model = !sideNav.model' class='hidden-md-and-up ml-3'></v-toolbar-side-icon>
      <v-toolbar-title>
        <nuxt-link to='/'><img src='/logo.png' class='myLogo' /></nuxt-link>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-spacer></v-spacer>
      <v-layout>
        <v-flex class='hidden-sm-and-down'>
          <v-btn to='#' dark flat>FEATURED COURSES</v-btn>
          <v-btn to='#' flat dark>LIBRARY</v-btn>
          <v-btn dark to='#' flat>LEARNING</v-btn>
          <v-btn dark to='#' flat>CHALLENGE</v-btn>
        </v-flex>
        <v-spacer></v-spacer>
        <v-spacer></v-spacer>
        <v-spacer></v-spacer>
        <v-spacer></v-spacer>
        <v-spacer></v-spacer>
        <v-spacer></v-spacer>
        <v-spacer></v-spacer>
        <v-flex class='hidden-sm-and-down'>
          <v-btn round class="px-4" outline to='/'>Log Out</v-btn>
        </v-flex>
      </v-layout>
    </v-toolbar>
    <nuxt></nuxt>
  </v-app>
</template>

<style lang='scss' scoped>
  a {
    text-decoration: none;
  }

  .myLogo {
    width: 100px;
    height: 70px;
    @media only screen and (max-width: 425px) {
      width: 50px;
      height: 30px;
      position: absolute;
      right: 36px;
      top: 38%;
    }
    @media only screen and (max-width: 959px) {
      width: 70px;
      height: 50px;
      position: absolute;
      right: 36px;
      top: 32%;
    }
  }

  .mobileLogo {
    @media only screen and (max-width: 800px) {
      display: none;
    }
  }

  .v-btn:hover:before,
  .v-btn:focus:before {
    border-bottom: solid white !important;
    background-color: unset;
  }

  .v-btn--active:before {
    background-color: unset;
  }

  .v-btn {
    font-weight: bolder;
    border-radius: 0 25px;
  }

  .profile-image {
    margin: 20% 0 15% 0;
  }

  .profile-image-holder {
    -webkit-box-shadow: -2px 10px 110px -16px rgba(204, 209, 237, 1);
    -moz-box-shadow: -2px 10px 110px -16px rgba(204, 209, 237, 1);
    box-shadow: -2px 10px 110px -16px rgba(204, 209, 237, 1);
  }
</style>

<script>
  export default {
    data() {
      return {
        sideNav: {
          model: false,
          type: 'persistent',
          clipped: false,
          floating: false,
          mini: false,
          stateless: true,
          scrolled: false
        }
      }
    }
  }
</script>
