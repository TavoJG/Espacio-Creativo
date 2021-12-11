<template>
  <v-row>
    <v-col cols="4">
      <v-row>
        <v-col cols="12">
          <v-card :height="cardHeight">
            <v-card-title>Misión</v-card-title>
            <v-card-text
              >Espacio creativo 4.0 tiene como misión ofrecer un espacio
              colaborativo al alcance de todos con infraestructura de la
              industria 4.0 que permita a los clientes crear proyectos de
              innovación, desarrollando nuevos conocimientos y habilidades para
              su crecimiento personal y profesional.</v-card-text
            >
          </v-card>
        </v-col>
        <v-col cols="12">
          <v-card :height="cardHeight">
            <v-card-title>Visión</v-card-title>
            <v-card-text
              >Ser el Makerspace líder en Latinoamérica impulsando la
              innovación, el ingenio y la creatividad a través de tecnologías
              nuevas, existentes y emergentes ofreciendo una infraestructura de
              primer nivel en un entorno colaborativo e inclusivo.</v-card-text
            >
          </v-card>
        </v-col>
      </v-row>
    </v-col>
    <v-col cols="8">
      <v-card height="425px">
        <v-card-title>Valores</v-card-title>
        <ValoresCarousel />
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
import { Component, Vue } from 'vue-property-decorator'

@Component({
  head:{
    title: "Acerca de nosotros"
  }
})
export default class About extends Vue {
  cardHeight = '200px'
}
</script>

