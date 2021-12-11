<template>
  <v-carousel v-model="model" hide-delimiters height="350">
    <v-carousel-item v-for="(valor, i) in valores" :key="i">
      <v-card elevation="0" height="350">
        <v-img
          :src="valor.imageLink"
          height="200px"
        />
        <v-card-title>{{ valor.titulo }}</v-card-title>
        <v-card-text>{{ valor.descripcion }}</v-card-text>
      </v-card>
    </v-carousel-item>
  </v-carousel>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'

interface Valor{
    titulo: string;
    descripcion: string;
    imageLink: string;
}

@Component
export default class extends Vue {
  model = 0
  valores:Valor[] = [
    {
      titulo: 'Respeto',
      descripcion: `Permite reconocer, aceptar, apreciar y valorar las cualidades de las demás personas,
así como sus derechos.`,
      imageLink: 'https://cdn.vuetifyjs.com/images/cards/sunshine.jpg',
    },
    {
      titulo: 'Responsabilidad',
      descripcion: `Dar cumplimiento a las obligaciones, cuidar de la comunidad de espacio
creativo 4.0 y asumir las consecuencias de las acciones.`,
imageLink: 'https://cdn.pixabay.com/photo/2019/12/14/18/28/sunrise-4695484_960_720.jpg',
    },
    {
      titulo: 'Honestidad',
      descripcion: `Deberá existir un comportamiento transparente, íntegro y de lealtad a la
organización, comprometiéndose con las políticas, normas y procedimientos.`,
imageLink: 'https://cdn.pixabay.com/photo/2013/07/18/20/26/sea-164989_960_720.jpg',
    },
    {
      titulo: 'Equidad',
      descripcion: `Crear y ofrecer condiciones que favorezcan la igualdad de oportunidades entre
todas las personas, para que sean parte de la comunidad en forma igualitaria, con respeto y
autonomía.`,
imageLink: 'https://cdn.pixabay.com/photo/2015/04/23/22/00/tree-736885_960_720.jpg'
    },
    {
      titulo: 'Colaboración',
      descripcion: `Trabajar en conjunto con otra u otras personas en la realización de proyectos
sin dejar de lado los valores de Espacio creativo 4.0.`,
imageLink: 'https://cdn.pixabay.com/photo/2016/11/08/05/20/sunset-1807524_960_720.jpg',
    },
  ]
}
</script>