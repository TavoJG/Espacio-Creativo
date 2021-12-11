<template>
  <video-player src="/avance1.mp4"/>
</template>

<script>
import { Component, Vue } from 'vue-property-decorator'
import VideoPlayer from 'nuxt-video-player'

require('nuxt-video-player/src/assets/css/main.css')

@Component({
  VideoPlayer,
})
export default class MainVideo extends Vue {}
</script>

