<template>
  <div id="home">
    <div class="wrapper-desc">
      <div class="card-project">
      <div class="capsule">
        <div class="wrapper">
<div class="desc">Eugene Fedotov</div>
        <div class="desc" style="text-align:center"><span class="uppercase subject">hacker - creator</span></div>
        <div class="center">
          <router-link to="/projects" class="uppercase hero-cta">learn about Eugene</router-link></div>
        </div>
      </div>
    </div>
        
    </div>
    <video id="hero" autoplay="autoplay" loop="loop" muted="muted">
        <source src="@/assets/hero.webm" type="video/webm">
        <source src="@/assets/hero.mp4" type="video/mp4">
    </video>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

export default class Home extends Vue {}
</script>

<style lang="scss" scoped>
#home {
  #hero {
    position: fixed;
    top: -30vh;
    right: 0;
    min-width: 100%;
    min-height: 100%;
    z-index: -1;
  }
  .wrapper-desc {
    z-index: 1;
    position: absolute;
    top:100px;
    font-size: 2rem;
    .card-project {
    background: #2e3138;
    box-shadow: 0 0 15px 1px rgba(0, 0, 0, 0.7);
    border: 1px solid #383b42;
    border-radius: 15px;
    opacity: 1;
    color: #c6d4df;
    margin: 20px 10px;
    padding:30px;
    }
  }
  .hero-cta{
        font-size: 24px;
            padding: 1em 1.5em 1em 2em;
    letter-spacing: 1.9px;
    font-weight: 400;
    min-width: 112px;
    outline: 0;
    white-space: normal;
    display: inline-block;
    text-decoration: none;
    line-height: 1em;
    vertical-align: middle;
    font-weight: 400;
    border-radius: 2px;
    user-select: none;
    text-align: center;
    border: solid #FF2643;
    overflow: visible;
    color: #FF2643;
    // background-color: #FF2643;
    background-color:transparent;
font-family: 'Helvetica Neue',Helvetica,Arial,sans-serif;
cursor:pointer;
margin-top:15px;
  }
}
.center{
  text-align: center;
}
</style>
