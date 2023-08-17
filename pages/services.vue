<template>
  <section>
    <h2
      class="text-h4 text-md-h3 text-center font-weight-black text-capitalize"
    >
      Explora Nuestras Soluciones
    </h2>
    <v-row no-gutters class="flex-row-reverse">
      <v-col cols="12" md="6" align-self="center">
        <v-img
          class="responsive-image"
          :src="solution1.image"
          :lazy-src="solution1.image"
        >
        </v-img>
      </v-col>
      <v-col cols="12" md="6" align-self="center">
        <div class="pa-lg-16 pa-md-10 px-4 py-16">
          <h2 class="text-h3 text-center font-weight-black">
            {{ solution1.title }}
          </h2>
          <h3 class="text-h5 text-uppercase font-weight-thin text-center my-8">
            {{ solution1.subtitle }}
          </h3>
          <p>"{{ solution1.description }}"</p>
        </div>
      </v-col>
    </v-row>
    <v-row no-gutters>
      <v-col cols="12" md="6" align-self="center">
        <v-img
          class="responsive-image"
          :src="solution2.image"
          :lazy-src="solution2.image"
        >
        </v-img>
      </v-col>
      <v-col cols="12" md="6" align-self="center">
        <div class="pa-lg-16 pa-md-10 px-4 py-16">
          <h2 class="text-h3 text-center font-weight-black">
            {{ solution2.title }}
          </h2>
          <h3 class="text-h5 text-uppercase font-weight-thin text-center my-8">
            {{ solution2.subtitle }}
          </h3>
          <p>"{{ solution2.description }}"</p>
        </div>
      </v-col>
    </v-row>
    <v-row no-gutters class="flex-row-reverse">
      <v-col cols="12" md="6" align-self="center">
        <v-img
          class="responsive-image"
          :src="solution3.image"
          :lazy-src="solution3.image"
        >
        </v-img>
      </v-col>
      <v-col cols="12" md="6" align-self="center">
        <div class="pa-lg-16 pa-md-10 px-4 py-16">
          <h2 class="text-h3 text-center font-weight-black">
            {{ solution3.title }}
          </h2>
          <h3 class="text-h5 text-uppercase font-weight-thin text-center my-8">
            {{ solution3.subtitle }}
          </h3>
          <p>"{{ solution3.description }}"</p>
        </div>
      </v-col>
    </v-row>
  </section>
</template>

<script>
export default {
  data() {
    return {
      solution1: {
        title: 'IntelliDent',
        subtitle: 'Aplicación para la detección de caries',
        description:
          '"Intellident" es una innovadora aplicación móvil para odontólogos, disponible en dispositivos Android 7 y superiores. Con tecnología de inteligencia artificial y visión por computadora, permite un análisis preciso de radiografías periapicales para detectar caries. Además, ofrece una completa gestión de pacientes y un odontograma para un seguimiento detallado de tratamientos. Potencia tu práctica odontológica con Alcance y diagnósticos más precisos.',
        image: 'intellident.png',
      },
      solution2: {
        title: 'TimeTrack Mobile',
        subtitle: 'Aplicación para el registro de asistencia',
        description:
          '"TimeTrack Mobile" es una innovadora aplicación móvil diseñada para el registro de asistencia de manera eficiente y segura. Dirigida especialmente a trabajadores de campo, TimeTrack utiliza tecnologías avanzadas como el geofencing y el reconocimiento facial para garantizar la precisión en el registro de entrada y salida de los empleados.',
        image: 'timetrack.png',
      },
      solution3: {
        title: 'TimeTrack Web',
        subtitle:
          'Gestión Centralizada TimeTrack: Control de Empleados y Horarios en la Web',
        description:
          'La versión web de TimeTrack es una plataforma administrativa integral diseñada para optimizar la gestión de empleados, horarios, trabajos y zonas en tu organización. Con TimeTrack Web, los administradores y supervisores pueden tener un control total sobre las operaciones laborales, permitiendo una administración eficiente y precisa de los recursos humanos y las actividades laborales.',
        image: 'timetrack-web.png',
      },
    }
  },
}
</script>
<style scoped>
.responsive-image {
  max-width: 100%;
  height: auto;
}
</style>
