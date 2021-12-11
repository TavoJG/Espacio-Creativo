<template>
  <v-row dense>
    <v-col cols="2">
      <v-card>
        <v-img
          src="/espacio_creativo.png"
          class="white--text align-end"
          gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
        />
      </v-card>
    </v-col>
    <v-col cols="5">
      <v-card>
        <v-card-title
          >Colabora, crea e innova en Espacio Creativo 4.0</v-card-title
        >
        <v-card-text
          >Espacio creativo 4.0 ofrece la renta de un espacio físico con
          infraestructura, recursos, herramientas, maquinaria y ambiente de la
          industria 4.0. Se podrá desarrollar proyectos de fabricación asistida,
          aditiva, manufactura, robótica y electrónica.</v-card-text
        >
      </v-card>
    </v-col>
    <v-col cols="5">
      <v-card>
        <v-card-title>Nuestra propuesta</v-card-title>
        <v-card-text
          >Espacio creativo 4.0 se constituirá por las áreas de fabricación
          aditiva, madera y metalmecánica, electrónica y robótica, centro de
          cómputo, corte laser y espacio para almacenamiento, también se contará
          con salones y áreas comunes.</v-card-text
        >
      </v-card>
    </v-col>
    <v-col cols="12">
      <ImageCarousel />
    </v-col>
  </v-row>
</template>

<script>
import { Component, Vue } from 'vue-property-decorator'

@Component({
  head:{
    title: "Página principal"
  }
})
export default class Index extends Vue {}
</script>

