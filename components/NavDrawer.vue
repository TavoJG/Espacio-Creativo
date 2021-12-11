<template>
  <v-navigation-drawer expand-on-hover permanent app>
    <v-list>
      <v-list-item
        v-for="(item, i) in items"
        :key="i"
        :to="item.to"
        router
        exact
      >
        <v-list-item-action>
          <v-icon>{{ item.icon }}</v-icon>
        </v-list-item-action>
        <v-list-item-content>
          <v-list-item-title v-text="item.title" />
        </v-list-item-content>
      </v-list-item>
    </v-list>
  </v-navigation-drawer>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'

@Component
export default class NavDrawer extends Vue {
  items = [
    {
      icon: 'mdi-home',
      title: 'Página principal',
      to: '/',
    },
    {
      icon: 'mdi-information-outline',
      title: 'Acerca de nosotros',
      to: '/about',
    },
    {
      icon: 'mdi-phone',
      title: 'Contacto',
      to: '/contacto',
    }
  ]
}
</script>

<style scoped>
</style>