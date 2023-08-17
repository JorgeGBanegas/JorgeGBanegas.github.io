<template>
  <section>
    <v-row no-gutters>
      <v-col cols="12">
        <SectionsHeroAlt :hero-alt="heroAlt" />
        <v-container>
          <v-row class="py-16">
            <v-col cols="12">
              <h2
                class="text-h4 text-md-h3 text-center font-weight-black text-capitalize"
              >
                Quiénes Somos?
              </h2>
              <h3
                class="text-h4 text-uppercase font-weight-thin text-center my-8"
              >
                Impulsando el Futuro con Innovación
              </h3>
            </v-col>
            <v-col cols="12" md="6">
              <p>
                En CodeMinds, somos un equipo apasionado de profesionales que se
                dedican a la creación de soluciones tecnológicas excepcionales.
                Nuestra empresa se fundó con la firme convicción de que la
                tecnología puede ser una fuerza positiva y transformadora en la
                sociedad.
              </p>
              <blockquote class="text-h4 pa-5 my-4 font-weight-thin">
                Guiados por nuestra pasión por la innovación y el compromiso con
                la excelencia, nos esforzamos por superar constantemente los
                estándares de calidad en todo lo que hacemos.
              </blockquote>
              <p>
                Nuestro objetivo es liderar la vanguardia de la industria
                tecnológica, forjando soluciones que no solo cumplan con las
                expectativas, sino que también inspiren un cambio positivo en la
                forma en que las personas interactúan con la tecnología en su
                vida diaria. Visualizamos un futuro en el que nuestras
                soluciones sean reconocidas por su capacidad para fomentar la
                inclusión, impulsar la sostenibilidad y reforzar la seguridad en
                la sociedad.
              </p>
            </v-col>
            <v-col cols="12" md="6">
              <p>
                En CodeMinds, nos esforzamos por construir un mundo en el que la
                tecnología avance en armonía con las necesidades y aspiraciones
                humanas. Estamos comprometidos con la excelencia y con marcar
                una diferencia duradera en la forma en que las personas
                experimentan y se benefician de la tecnología.
              </p>
            </v-col>
          </v-row>
        </v-container>

        <v-row no-gutters>
          <v-col cols="12" md="6" align-self="center">
            <v-img height="100vh" src="vision.jpg" lazy-src="vision.jpeg">
            </v-img>
          </v-col>
          <v-col cols="12" md="6" align-self="center">
            <div class="pa-lg-16 pa-md-10 px-4 py-16">
              <h2 class="text-h3 text-center font-weight-black">
                Nuestra Visión
              </h2>
              <h3
                class="text-h5 text-uppercase font-weight-thin text-center my-8"
              >
                Iluminando el Futuro Tecnológico con Innovación y Pasión
              </h3>
              <p>
                "Visualizamos a CodeMinds como un faro de innovación en el
                horizonte tecnológico. Nuestra ambición es extender nuestras
                raíces a lo largo de múltiples países de Sudamérica, tejiendo
                una red de soluciones de software que trasciendan las
                expectativas. Con un enfoque en la inteligencia artificial,
                aspiramos a tejer lazos entre la tecnología y la humanidad,
                empoderando a comunidades diversas, protegiendo nuestro entorno
                y estableciendo nuevos estándares de seguridad y bienestar."
              </p>
            </div>
          </v-col>
        </v-row>
        <v-row no-gutters class="flex-row-reverse">
          <v-col cols="12" md="6" align-self="center">
            <v-img height="100vh" src="mision.jpg" lazy-src="mision.jpg">
            </v-img>
          </v-col>
          <v-col cols="12" md="6" align-self="center">
            <div class="pa-lg-16 pa-md-10 px-4 py-16">
              <h2 class="text-h3 text-center font-weight-black">
                Nuestra Misión
              </h2>
              <h3
                class="text-h5 text-uppercase font-weight-thin text-center my-8"
              >
                Innovar con Excelencia Tecnológica
              </h3>
              <p>
                "La misión de CodeMinds es desarrollar soluciones de software
                excepcionales que establezcan nuevos estándares de calidad y
                creatividad. Nos guían la responsabilidad, la puntualidad y la
                colaboración, con el objetivo de ser reconocidos como una
                empresa innovadora que ofrece productos tecnológicos de primera
                categoría y a la vanguardia."
              </p>
            </div>
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </section>
</template>

<script>
export default {
  data() {
    return {
      heroAlt: [
        {
          src: 'pexels-moose-photos-1036641.jpg',
          heading: 'SOBRE NOSOTROS',
        },
      ],
    }
  },
  head() {
    return {
      title: 'SOBRE NOSOTROS',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content:
            'Infographic hypotheses influencer user experience Long madel ture gen-z paradigm shift client partner network product seilans solve management influencer analytics leverage virality. incubator seed round massmarket. buyer agile development growth hacking business-to-consumer ecosystem',
        },
      ],
    }
  },
}
</script>
