<template>
  <div class="home">
    <video id="hero" autoplay="autoplay" loop="loop" muted="muted">
        <source src="@/assets/hero.webm" type="video/webm">
        <source src="@/assets/hero.mp4" type="video/mp4">
    </video>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import HelloWorld from '@/components/HelloWorld.vue'; // @ is an alias to /src

@Component({
  components: {
    HelloWorld,
  },
})
export default class Home extends Vue {}
</script>

<style lang="scss">
#hero {
    position: fixed;
    right: 0;
    bottom: 0;
    min-width: 100%; 
    min-height: 100%;
}
</style>
