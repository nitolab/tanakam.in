<template>
  <div>
    <MainHeader/>

    <div class="wrp">
      <section class="hero is-medium is-primary is-bold">
        <div class="hero-body">
          <div class="container">
            <h1 class="title">
              高波
            </h1>
          </div>
        </div>
      </section>

      <div class="container">
        <article>
          <p>絶賛テスト中</p>
        </article>
      </div>
    </div>
    <Footer/>
  </div>
</template>

<script>
import MainHeader from '~/components/MainHeader'
import Footer from '~/components/Footer'
export default {
  components: {
    MainHeader,
    Footer
  },
  head () {
    return {
      title: 'takanami',
      meta: [
        { hid: 'twitter:card', name: 'twitter:card', content: 'summary' },
        // { hid: 'twitter:creator', name: 'twitter:creator', content: '@' },
        { hid: 'og:url', name: 'og:url', content: process.env.siteUrl+this.$route.fullPath },
      ]
    }
  },
}
</script>

<style>
</style>
