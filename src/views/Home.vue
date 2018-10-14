<template>
  <div id="home">
    <div class="header">

      <video id="hero" autoplay="autoplay" loop="loop" muted="muted">
        <source src="@/assets/hero.webm" type="video/webm">
        <source src="@/assets/hero.mp4" type="video/mp4">
      </video>
      <div class="wrapper-desc">
        <div class="desc">Eugene Fedotov</div>
        <div class="desc" style="text-align:center"><span class="uppercase subject">hacker - creator</span></div>
        <div class="center">
          <router-link to="/projects" class="uppercase hero-cta">learn more</router-link>
        </div>
      </div>
    </div>
    <div class="about-container">
      <div class="avatar-container">
        <img class="avatar" src="https://github.com/eugenefedoto.png" alt="">
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Vue } from "vue-property-decorator";

export default class Home extends Vue {}
</script>

<style lang="scss" scoped>
#hero {
  width: 100%;
  position: relative;
  z-index: -1;
}
.avatar-container {
  display: flex;
  justify-content: center;
  .avatar {
    border-radius: 50%;
    height: 200px;
  }
}
.wrapper-desc {
  z-index: 1;
  position: absolute;
  top: 10vh;
  font-size: 2rem;
  background: #2e3138;
  box-shadow: 0 0 15px 1px rgba(0, 0, 0, 0.7);
  border: 1px solid #383b42;
  border-radius: 15px;
  color: #c6d4df;
  margin: 1rem;
  padding: 1rem;
  opacity: 0.9;
  top: 10vh;
}
.hero-cta {
  padding: 0.5em;
  letter-spacing: 1.9px;
  font-weight: 400;
  outline: 0;
  white-space: normal;
  display: inline-block;
  text-decoration: none;
  vertical-align: middle;

  border-radius: 2px;
  user-select: none;
  text-align: center;
  border: solid #ff2643;
  overflow: visible;
  color: #ff2643;
  background-color: transparent;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  cursor: pointer;
}

.center {
  text-align: center;
  display: flex;
  justify-content: space-evenly;
  margin: 10px;
}
.desc {
  text-align: center;
}
.subject {
  display: inline-block;
  line-height: 1.2em;
}
@media only screen and (max-width: 768px) {
  .wrapper-desc {
    font-size: 2rem;
    // padding: 0.5rem;
  }
  .header {
    display: flex;
    justify-content: center;
    flex-direction: column;
  }
  video {
  }
}
@media only screen and (max-width: 320px) {
  .wrapper-desc {
    font-size: 1rem;
    margin: 0;
    .hero-cta {
      display: none;
    }
  }
  .header {
    align-items: center;
  }
  .avatar-container {
    .avatar {
      height: 100px;
      z-index: 1;
    }
  }
}
</style>
