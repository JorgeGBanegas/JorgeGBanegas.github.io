<template>
  <section id="intro" class="py-16">
    <v-container>
      <v-responsive class="max-auto mx-auto text-center" max-width="600">
        <v-avatar color="primary" size="70" class="mb-8">
          <v-icon x-large dark>mdi-cogs</v-icon>
        </v-avatar>
        <h2 class="text-h4 text-md-h3 text-center font-weight-black mb-7">
          Impulsa tu Negocio con Soluciones Tecnológicas Avanzadas
        </h2>
        <p class="title font-weight-light">
          CodeMinds — te ofrece soluciones tecnológicas de vanguardia que
          aprovechan la inteligencia artificial, blockchain, IoT y más. Nuestros
          expertos en desarrollo te brindarán las herramientas necesarias para
          llevar tu negocio al siguiente nivel.
        </p>
      </v-responsive>

      <v-row class="pt-12">
        <v-col v-for="card in cards" :key="card.title" cols="12" md="4">
          <v-row no-gutters>
            <v-col :cols="card.callout ? 9 : 12">
              <div class="pr-2">
                <div class="text--disabled" v-text="card.subtitle"></div>
                <h4
                  class="text-uppercase mt-1 mb-4"
                  style="letter-spacing: 0.15em"
                  v-text="card.title"
                ></h4>
                <p v-text="card.text"></p>
              </div>
            </v-col>
            <v-col v-if="card.callout" cols="2">
              <span
                class="text-h3 grey--text font-weight-bold pr-8"
                style="opacity: 0.1"
                >{{ card.callout }}</span
              >
            </v-col>
          </v-row>
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
          title: 'Soluciones de IA',
          subtitle: 'Inteligencia Artificial',
          text: 'Desarrollamos aplicaciones y sistemas que utilizan la inteligencia artificial para automatizar tareas, tomar decisiones informadas y mejorar la eficiencia.',
          callout: '01',
        },
        {
          title: 'Innovación con Blockchain',
          subtitle: 'Tecnología de Blockchain',
          text: 'Exploramos las posibilidades del blockchain para crear soluciones seguras y transparentes en áreas como el suministro, la cadena de bloques y más.',
          callout: '02',
        },
        {
          title: 'Conectando el Mundo con IoT',
          subtitle: 'Internet de las Cosas',
          text: 'Creamos aplicaciones y plataformas que aprovechan el Internet de las Cosas para proporcionar conectividad y control en tiempo real.',
          callout: '03',
        },
      ],
    }
  },
}
</script>
