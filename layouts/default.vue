<template>
  <v-app dark>
    <siteHeader />
    <v-main>
      <nuxt />
      <footerTop />
    </v-main>
    <siteFooter />
    <Notification />
  </v-app>
</template>

<script>
import siteHeader from '~/components/siteHeader.vue'
import footerTop from '~/components/footerTop.vue'
import siteFooter from '~/components/siteFooter.vue'
export default {
  components: {
    siteHeader,
    footerTop,
    siteFooter,
  },
  mounted() {
    const id = process.env.NUXT_ENV_CHAT_ID
    const src = process.env.NUXT_ENV_CHAT_SRC
    // Configura el ID del chatbot proporcionado por Trypika
    window.pikaChatbotId = id

    // Crea un nuevo elemento script y configura sus atributos
    const scriptElement = document.createElement('script')
    scriptElement.src = src
    scriptElement.id = id
    scriptElement.defer = true

    // Agrega el elemento script al final del body para cargar el chatbot
    document.body.appendChild(scriptElement)
  },
  head() {
    return {
      script: [
        {
          src: 'https://www.googletagmanager.com/gtag/js?id=G-0DYDMZEYDZ',
        },
      ],
    }
  },
}
</script>

<style></style>
