<template>
  <div>
    <v-navigation-drawer v-model='sideNav.model' disable-resize-watcher width='200' app overflow left persistent>
      <v-list>
        <v-list-tile>
          <v-list-tile-action>
            <nuxt-link class="black--text" to='#'>
              <img src="/home_1.png" alt="">
            </nuxt-link>
          </v-list-tile-action>
          <v-list-tile-content>
            <nuxt-link class="black--text" to='#'>Home</nuxt-link>
          </v-list-tile-content>
        </v-list-tile>
        <v-list-tile>
          <v-list-tile-action>
            <nuxt-link class="black--text" to='#'>
              <img src="#_1.png" alt="">
            </nuxt-link>
          </v-list-tile-action>
          <v-list-tile-content>
            <nuxt-link class="black--text" to='#'>About</nuxt-link>
          </v-list-tile-content>
        </v-list-tile>
        <v-list-tile>
          <v-list-tile-action>
            <nuxt-link to='#'>
              <img src="/faq_1.png" alt="">
            </nuxt-link>
          </v-list-tile-action>
          <v-list-tile-content>
            <nuxt-link class="black--text" to='#'>LEARNING</nuxt-link>
          </v-list-tile-content>
        </v-list-tile>
        <v-list-tile>
          <v-list-tile-action>
            <nuxt-link to='#'>
              <img src="/faq_1.png" alt="">
            </nuxt-link>
          </v-list-tile-action>
          <v-list-tile-content>
            <nuxt-link class="black--text" to='#'>CHALLENGE</nuxt-link>
          </v-list-tile-content>
        </v-list-tile>
        <v-list-tile>
          <v-list-tile-action>
            <nuxt-link to='#'>
              <img src="/signup_1.png" alt="">
            </nuxt-link>
          </v-list-tile-action>
          <v-list-tile-content>
            <nuxt-link class="black--text" to='#'>Sign Up</nuxt-link>
          </v-list-tile-content>
        </v-list-tile>
        <v-list-tile>
          <v-list-tile-action>
            <nuxt-link to='#'>
              <img src="/login_1.png" alt="">
            </nuxt-link>
          </v-list-tile-action>
          <v-list-tile-content>
            <nuxt-link class="black--text" to='#'>Sign In</nuxt-link>
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
          <v-btn to='#' dark flat>Home</v-btn>
          <v-btn to='#' flat dark>About</v-btn>
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
          <v-btn dark flat to='#'>Sign Up</v-btn>
          <v-btn round class="px-4" outline to='#'>Log In</v-btn>
        </v-flex>
      </v-layout>
    </v-toolbar>
    <main>

    </main>
  </div>
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
</style>


<script>
  export default {
    data: () => ({
      sideNav: {
        model: false,
        type: 'persistent',
        clipped: false,
        floating: false,
        mini: false,
        stateless: true,
        scrolled: false
      }
    })
  }
</script>
