<template>
    <v-app light>
      <Header></Header>
        <nuxt></nuxt>
    </v-app>
</template>

 <script>
import Header from '@/components/header'
import Footer from '@/components/footer'
export default {
  data () {
    return {

    }
  },
  components: {
    Footer,
    Header
  }
}
</script>
