<template>
  <section :class="$vuetify.theme.dark ? 'black' : 'white'" class="py-16">
    <v-container>
      <v-row>
        <v-col>
          <v-row no-gutters>
            <v-col class="text-center">
              <h2
                class="text-h4 text-md-h3 text-center font-weight-black text-capitalize mb-4"
              >
                Precios de Soluciones de Software
              </h2>

              <p class="my-10 title">
                En CodeMinds, ofrecemos una variedad de soluciones de software
                innovadoras para satisfacer sus necesidades. Desde aplicaciones
                personalizadas hasta soluciones basadas en suscripción, tenemos
                opciones para todas las empresas. Explora nuestras soluciones y
                elige la que mejor se adapte a tu negocio.
              </p>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
    <v-container fluid>
      <v-row class="mx-auto" style="max-width: 1200px">
        <v-col
          v-for="(solution, index) in solutions"
          :key="`solution-${index}`"
          cols="12"
          md="4"
        >
          <v-hover v-slot="{ hover }">
            <v-card
              :elevation="hover ? 24 : solution.elevation"
              :color="solution.color"
              max-width="400"
              :class="hover ? 'zoom' : 'notzoom'"
              class="mx-auto transition-swing"
            >
              <h3
                class="text-h4 text-center font-weight-black white--text pt-5"
                v-text="solution.name"
              ></h3>
              <v-card-text
                class="text-center subtitle-1 white--text py-2"
                v-text="solution.description"
              ></v-card-text>
              <v-card-subtitle
                class="text-h5 font-weight-black text-center white--text pt-0"
              >
                {{ solution.pricing }}
              </v-card-subtitle>
              <v-list>
                <v-list-item
                  v-for="(feature, ik) in solution.features"
                  :key="`feature-${ik}`"
                  dense
                >
                  <v-list-item-icon>
                    <v-icon>
                      {{ feature.icon }}
                    </v-icon>
                  </v-list-item-icon>
                  <v-list-item-content>
                    <v-list-item-title
                      class="text-capitalize"
                      v-text="feature.text"
                    ></v-list-item-title>
                  </v-list-item-content>
                </v-list-item>
                <v-list-item>
                  <v-btn
                    color="primary"
                    large
                    block
                    rounded
                    class="mx-auto my-3"
                  >
                    Obtener Más Información
                  </v-btn>
                </v-list-item>
              </v-list>
            </v-card></v-hover
          >
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<script>
export default {
  data() {
    return {
      solutions: [
        {
          name: 'Solución de Reconocimiento Facial',
          elevation: 0,
          color: 'primary darken-1',
          description: 'Desarrollo de aplicación con IA',
          pricing: 'Precio: Consultar',
          features: [
            {
              icon: 'mdi-face-recognition',
              text: 'Tecnología avanzada de reconocimiento facial',
            },
            {
              icon: 'mdi-lock',
              text: 'Seguridad y privacidad mejoradas',
            },
            {
              icon: 'mdi-database-search',
              text: 'Análisis y estadísticas detalladas',
            },
            {
              icon: 'mdi-cloud-sync',
              text: 'Integración en la nube',
            },
          ],
        },
        {
          name: 'Solución de IoT Personalizada',
          elevation: 16,
          color: 'green darken-2',
          description: 'Desarrollo de aplicación para IoT',
          pricing: 'Precio: Consultar',
          features: [
            {
              icon: 'mdi-wifi',
              text: 'Conectividad y control remoto',
            },
            {
              icon: 'mdi-temperature-celsius',
              text: 'Monitoreo y análisis de datos en tiempo real',
            },
            {
              icon: 'mdi-cogs',
              text: 'Integración de sensores y dispositivos',
            },
            {
              icon: 'mdi-clock-time-three-outline',
              text: 'Automatización y programación',
            },
          ],
        },
        {
          name: 'Solución de Blockchain Innovadora',
          elevation: 0,
          color: 'orange darken-3',
          description: 'Desarrollo de aplicación basada en blockchain',
          pricing: 'Precio: Consultar',
          features: [
            {
              icon: 'mdi-chain',
              text: 'Tecnología de registro distribuido',
            },
            {
              icon: 'mdi-lock-alert',
              text: 'Seguridad y confiabilidad de datos',
            },
            {
              icon: 'mdi-link-box-outline',
              text: 'Transparencia y trazabilidad',
            },
            {
              icon: 'mdi-handshake',
              text: 'Intercambio seguro y verificable',
            },
          ],
        },
      ],
    }
  },
}
</script>

<style scoped>
.zoom {
  transform: scale(1.025) translate(0, -10px);
  transition: transform 0.2s;
}

.notzoom {
  transition: transform 0.2s;
}
</style>
