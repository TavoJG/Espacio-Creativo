<template>
  <v-footer app padless>
    <v-card flat tile class="white--text text-center" width="100%">
      <v-card-text>
        <v-btn
          v-for="icon in icons"
          :key="icon"
          class="mx-4 white--text"
          icon
          :href="icon.url"
        >
          <v-icon size="24p">
            {{ icon.name }}
          </v-icon>
        </v-btn>
      </v-card-text>
      <v-card-text class="white--text"
        >&copy;{{ new Date().getFullYear() }} -
        <strong>Espacio Creativo 4.0</strong>
      </v-card-text>
    </v-card>
  </v-footer>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'

interface IconLink {
  name: string
  url: string
}

@Component
export default class extends Vue {
  icons: IconLink[] = [
    {
      name: 'mdi-facebook',
      url: 'https://www.facebook.com/EspacioCreativo4.0Mex',
    },
    {
      name: 'mdi-instagram',
      url: 'https://www.instagram.com/espaciocreativo4.0/?hl=es',
    },
  ]
}
</script>

<style scoped>
</style>