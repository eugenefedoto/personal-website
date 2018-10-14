<template>
  <div id="app">
    <nav class="site-nav site-nav--home" :class="{'is-open-accordion': isOpenAccordion}">
      <div class="section-contained-narrow site-nav__container">
        <div class="site-nav__main">
          <div class="site-nav__menu-item visible-md" v-on:click="openAccordion">
            <div class="site-nav__block">
              <button class="site-nav-hamburger" type="button">
                <span class="site-nav-hamburger___inner"></span>
              </button>
            </div>
          </div>
          <div class="site-nav__logo">
            <router-link to="/" class="site-nav__link nav-link-underline">
              ef_
            </router-link>
          </div>
          <div class="site-nav-accordion">
            <div class="site-nav__menu-item">
              <router-link to="/projects" class="site-nav__link nav-link-underline" v-on:click.native="isOpenAccordion = false">
                <div class="site-nav__block">
                  <div class="site-nav-item__name">Projects</div>
                </div>
              </router-link>
            </div>
          </div>
        </div>
      </div>
    </nav>
    <router-view />
  </div>
</template>

<script lang='ts'>
import Vue from "vue";
export default Vue.extend({
  data() {
    return {
      isOpenAccordion: false,
    };
  },
  methods: {
    openAccordion() {
      this.isOpenAccordion = !this.isOpenAccordion;
    },
  },
});
</script>


<style lang="scss">
@import "~normalize.css";

* {
  -webkit-font-smoothing: antialiased;
  font-family: "Source Sans Pro", "Helvetica Neue", Helvetica, Arial, sans-serif;

  -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
  font-weight: 300;
}

body {
  background: black;
}

.wrapper-nav {
  font-family: Nobile, sans-serif;
  font-size: 2rem;
  display: flex;
  margin-top: 5vh;
  margin-left: 1vw;
  #logo {
    margin: 0 2vw;
  }
  .tabs {
    font-size: 1.1rem;
    background: #e2e2e2;
    box-shadow: 0.1rem 0.1rem 0.3rem rgba(0, 0, 0, 0.1);
    border-radius: 0 1rem 1rem 0;
    a {
      text-decoration: none;
      color: #777;
      text-transform: uppercase;
      padding: 0.5em;
      display: inline-block;
      &:hover {
        color: #ff006a;
      }
    }
  }
}
.subject,
.site-nav__logo a {
  text-decoration: none;
  background: linear-gradient(to right, #30cfd0 0%, #6410cc 100%);
  background-clip: text;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-size: 24px;
}
.site-nav__logo {
  a {
    margin-left: 15px;
  }
}
.desc {
  font-size: 2em;
  color: white;
  .subject {
    font-size: 0.6em;
  }
}
.uppercase {
  text-transform: uppercase;
}
.site-nav--home {
  transition: all 200ms ease-in-out;
  border-bottom: none;
  background-color: rgba(0, 0, 0, 0.8);
}
@media only screen and (max-width: 480px) {
  .site-nav__container {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
  }
}

.section-contained-narrow {
  margin: 0 auto;
  width: 100%;
}
.site-nav__main,
.site-nav__secondary,
.site-nav__settings,
.site-nav__logo {
  display: flex;
  flex-direction: row;
  align-items: center;
  height: 47px;
}

@media only screen and (max-width: 768px) {
  .site-nav__block {
    font-size: 14px;
  }
  .site-nav-accordion .site-nav__block {
    text-align: center;
    display: block;
  }
}
.site-nav__block {
  display: flex;
  flex-direction: row;
  align-items: center;
  position: relative;
}
.site-nav-hamburger {
  margin: 5px 5px;
  display: inline-block;
  position: relative;
  cursor: pointer;
  transition: opacity, filter 150ms linear;
  width: 20px;
}
button {
  background: none;
  border: none;
  border-radius: 0;
}
a,
button {
  text-decoration: none;
  color: #2e9fff;
}
.site-nav-hamburger___inner,
.site-nav-hamburger___inner:before,
.site-nav-hamburger___inner:after {
  width: 20px;
  height: 3px;
  background-color: #54aeff;
  border-radius: 4px;
  position: absolute;
  content: "";
  display: block;
}
.site-nav-hamburger___inner {
  top: 50%;
  margin-top: -1px;
  transition: 100ms cubic-bezier(0.55, 0.055, 0.675, 0.19);
}
.site-nav--home .site-nav__logo {
  position: relative;
  width: 110px;
  transition: all 200ms ease-in-out;
}

@media only screen and (max-width: 426px) {
  .is-open-accordion .site-nav-accordion {
    max-height: 500px;
  }
}
.no-touch a:hover,
.no-touch button:hover,
.no-touchevents a:hover,
.no-touchevents button:hover {
  color: #2e87e7;
}
.site-nav-hamburger:hover {
  opacity: 0.7;
}
.site-nav-hamburger___inner:before {
  top: -7px;
  transition: top 100ms 140ms ease, opacity 100ms ease;
}
.site-nav-hamburger___inner:after {
  bottom: -7px;
  transition: bottom 100ms 140ms ease,
    transform 100ms cubic-bezier(0.55, 0.055, 0.675, 0.19);
}
.site-nav--home .logo--light {
  opacity: 0;
  visibility: hidden;
}
.site-nav--home .logo {
  position: absolute;
  top: 14px;
  transition: opacity 250ms ease-in-out;
}
.site-nav img,
.site-nav svg {
  display: block;
}
.logo {
  height: 20px;
  width: 110px;
}
@media only screen and (min-width: 769px) {
  .site-nav-accordion {
    display: flex;
    flex-direction: row;
    align-items: center;
    height: 47px;
  }
}

@media only screen and (min-width: 768px) {
  .site-nav--marketing .site-nav__link {
    color: #54aeff;
  }
}

.site-nav__link {
  position: relative;
  text-align: center;
  display: block;
  transition: all 250ms ease-in-out;
}
@media screen and (min-width: 426px) {
  .visible-md {
    display: none !important;
  }
}
@media only screen and (min-width: 961px) {
  .site-nav__container {
    padding: 0;
  }
}
.site-nav__container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}

@media only screen and (min-width: 1026px) {
  .section-contained-narrow {
    max-width: 960px;
  }
}
.section-contained-narrow {
  margin: 0 auto;
  width: 100%;
}
html {
  overflow-y: scroll;
}
@media only screen and (max-width: 426px) {
  .site-nav-accordion .site-nav__link {
    padding-top: 15px;
    padding-bottom: 15px;
    background-color: #494e58;
    color: #c2c9d4;
    border-bottom: 1px solid #353a3d;
  }
  .site-nav-accordion {
    position: absolute;
    top: 50px;
    left: 0;
    right: 0;
    width: 100%;
    overflow-y: hidden;
    max-height: 0;
    transition: all 400ms ease-in-out;
  }
}
@media only screen and (max-width: 769px) {
  .is-open-accordion .site-nav-accordion {
    max-height: 500px;
  }
}
.site-nav-accordion {
  z-index: 2;
}
</style>
