<template>
  <v-carousel v-model="model">
    <v-carousel-item v-for="(image, i) in images" :key="i">
      <v-card>
        <v-img
          :src="buildImageSrc(image.imageName)"
          class="white--text align-end"
          gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
          height="500px"
        >
          <v-card-title v-text="image.title"></v-card-title>
        </v-img>
      </v-card>
    </v-carousel-item>
  </v-carousel>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'

interface Image {
  title: string
  imageName: string
}

@Component
export default class extends Vue {
  imageFolder = '/carousel'

  buildImageSrc(imageName: string): string {
    return `${this.imageFolder}/${imageName}`
  }

  model = 0
  images: Image[] = [
    {
      title: 'Torno CNC',
      imageName: 'cnc.png',
    },
    {
      title: 'Aulas modernas',
      imageName: 'aulas.png',
    },
    {
      title: 'Impresión aditiva',
      imageName: 'impresora3d.png',
    },
    {
      title: 'Laboratorio de electrónica',
      imageName: 'electronica.png',
    }
  ]
}
</script>
