<template>
  <v-app dark>
    <NavDrawer />
    <MainBar />
    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
    <MainFooter/>
  </v-app>
</template>

<script>
export default {
  data() {
    return {}
  },
}
</script>

<style scoped>
</style>
