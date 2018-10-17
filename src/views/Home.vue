<template>
  <div id="home">
    <div class="header">
      <video id="hero" autoplay="autoplay" loop="loop" muted="muted">
        <source src="@/assets/hero.webm" type="video/webm">
        <source src="@/assets/hero.mp4" type="video/mp4">
      </video>
      <div class="wrapper-desc">
        <div class="desc">Eugene Fedotov</div>
        <div class="desc"><span class="uppercase subject">hacker - creator</span></div>
        <div class="center">
          <a href="#about" class="uppercase hero-cta">learn more</a>
        </div>
      </div>
    </div>
    <div class="content">
      <div class="container">
        <div id="about" class="feature" style="display:flex;  flex-wrap:wrap;">
          <div id="avatar-container">
            <img class="avatar" src="https://github.com/eugenefedoto.png" alt="">
          </div>

          <ul>
            Hobbies
            <li>hacking</li>
            <li>programming</li>
            <li>anime</li>
            <li>gaming</li>
          </ul>
          <ul>
            Past Roles
            <li>Lead frontend development at Dell</li>
            <li>Developed Node.js services for APPrise Mobile.</li>
            <li>Converted web designs as a freelancer.</li>
          </ul>
          <div><a href="/Eugene_Fedotov_Resume.pdf">Resume</a></div>
          <div><a href="https://github.com/eugenefedoto">GitHub</a></div>

        </div>

        <div class="feature story">
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Vue } from "vue-property-decorator";

export default class Home extends Vue {}
</script>

<style lang="scss">
.feature {
  color: #7f8fad;
  font-size: 1.5rem;
  li,
  p {
    color: #596985;
  }
  p {
    font-size: 0.9em;
  }
  &.story {
    margin: 0 1rem;
    flex-wrap: wrap;
    h2 {
      flex: 0 0 100%;
      margin: 0.5em;
    }
    p {
      margin: 0.5em;
    }
  }
}
#hero {
  width: 100%;
  position: relative;
  z-index: -1;
}
.container {
  // display: flex;
  // text-align: center;
  .avatar {
    border-radius: 50%;
    height: 100px;
  }
}
.wrapper-desc {
  display: flex;
  justify-content: center;
  max-width: 500px;
  flex-wrap: wrap;
  z-index: 1;
  position: absolute;
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
// .desc {
//   text-align: center;
// }
.subject {
  display: inline-block;
  line-height: 1.2em;
}
@media only screen and (max-width: 769px) {
  .wrapper-desc {
    font-size: 2rem;
  }
}
@media only screen and (max-width: 426px) {
  .wrapper-desc {
    font-size: 1rem;
    margin: 0;
    border-radius: unset;
    .hero-cta {
      display: none;
    }
  }
  .header {
    align-items: center;
  }
  .container {
    .avatar {
      height: 100px;
      z-index: 1;
    }
  }
}
.feature {
  div {
    display: flex;
    flex: 0 0 100%;
    justify-content: center;
  }
}
@media only screen and (min-width: 767px) {
  .feature {
    display: flex;
    justify-content: center;
    #avatar-container {
      flex-basis: auto;
    }
  }
}
</style>
