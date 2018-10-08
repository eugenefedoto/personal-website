<template>
  <div id="home">
    <div class="wrapper-desc">
        <div class="desc">Eugene Fedotov</div>
        <div class="desc">is a <span class="uppercase subject">hacker</span></div>
        <div class="desc">is a <span class="uppercase subject">developer</span></div>
        <div class="desc">loves <span class="uppercase subject">anime</span></div>
    </div>
    <video id="hero" autoplay="autoplay" loop="loop" muted="muted">
        <source src="@/assets/hero.webm" type="video/webm">
        <source src="@/assets/hero.mp4" type="video/mp4">
    </video>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import HelloWorld from "@/components/HelloWorld.vue"; // @ is an alias to /src

@Component({
  components: {
    HelloWorld
  }
})
export default class Home extends Vue {}
</script>

<style lang="scss" scoped>
#home {
  #hero {
    position: fixed;
    right: 0;
    bottom: 0;
    min-width: 100%;
    min-height: 100%;
  }
  .wrapper-desc {
    z-index: 1;
    position: absolute;
    margin-top: 20vh;
    margin-left: 10vw;
    font-size: 2rem;
  }
}
</style>
