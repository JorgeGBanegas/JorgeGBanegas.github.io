<template>
  <section class="primary darken-1 white--text py-16">
    <v-container>
      <v-row>
        <v-col class="text-center">
          <h2 class="text-h4 text-md-h3 text-center font-weight-black">
            Potencia Tu Negocio con Tecnología de Vanguardia
          </h2>
          <div
            class="text-h5 text-md-h4 text-center font-weight-black py-3 mb-10"
          >
            ¡Explora Nuestras Soluciones y Desbloquea el Futuro!
          </div>
        </v-col>
      </v-row>
      <v-row>
        <v-col
          v-for="(card, index) in cards"
          :key="index"
          cols="12"
          sm="4"
          class="text-center"
        >
          <v-avatar
            size="80"
            class="display-1 white font-weight-bold primary--text mb-5"
            style="opacity: 1.15"
            >{{ card.callout }}</v-avatar
          >
          <div class="title text-uppercase mt-1 mb-4" v-text="card.title"></div>

          <p v-text="card.text"></p>
          <v-row no-gutters>
            <v-col cols="12"> </v-col>
          </v-row>
        </v-col>
      </v-row>
      <v-row no-gutters>
        <v-col cols="12" class="text-center">
          <router-link
            to="/services"
            tag="v-btn"
            x-large
            rounded
            color="primary"
            dark
            class="mx-auto mt-10 px-16"
          >
            <v-icon dark left>mdi-check-bold</v-icon> Explorar Soluciones
          </router-link>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<script>
export default {
  data() {
    return {
      cards: [
        {
          title: 'Soluciones Innovadoras',
          subtitle: 'Desbloquea Posibilidades',
          text: 'Aprovecha el poder de la Inteligencia Artificial, Blockchain, IoT y más para impulsar tu negocio hacia adelante.',
          callout: '01',
        },
        {
          title: 'Crecimiento Estratégico',
          subtitle: 'Maximiza el Potencial',
          text: 'Transforma tus operaciones con insights y estrategias basados en datos que conducen a un crecimiento sostenible.',
          callout: '02',
        },
        {
          title: 'Tecnología a Prueba de Futuro',
          subtitle: 'Mantente a la Vanguardia',
          text: 'Abraza el futuro con nuestras tecnologías de vanguardia que aseguran que tu negocio siga siendo competitivo y adaptable.',
          callout: '03',
        },
      ],
    }
  },
}
</script>
