<template>
  <v-layout align-start justify-center>
    <v-flex xs12 sm8 md4>
      <v-card class="elevation-12" dark>
        <v-img
          src="https://cdn.pixabay.com/photo/2016/03/10/09/24/typewriter-1248088_960_720.jpg"
          max-width="450"
          max-height="450"
          class="mx-auto"
        />
        <v-card-title>Contacto</v-card-title>

        <v-card-text
          >Próximamente podrás ponerte en contacto con nosotros. ¡Te
          esperamos!</v-card-text
        >
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>
import { Component, Vue } from 'vue-property-decorator'

@Component({
  head: {
    title: 'Contacto',
  },
})
export default class About extends Vue {}
</script>

