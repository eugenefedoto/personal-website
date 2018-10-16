<template>
  <div id="projects">
    <div class="" style="padding-top:47px">
      <picture>
        <source srcset="@/assets/personal-website.png" media="(max-width: 768px)">
        <img class="page active" src="@/assets/originals/personal-website.png">
      </picture>
      <picture>
        <source srcset="@/assets/love-you-forever.png" media="(max-width: 768px)">
        <img class="page active" src="@/assets/originals/love-you-forever.png">
      </picture>
      <picture>
        <source srcset="@/assets/bike-location-finder-v1.png" media="(max-width: 768px)">
        <img class="page active" src="@/assets/originals/bike-location-finder-v1.png">
      </picture>
      <picture>
        <source srcset="@/assets/bike-location-finder-v2.png" media="(max-width: 768px)">
        <img class="page active" src="@/assets/originals/bike-location-finder-v2.png">
      </picture>
      <picture>
        <source srcset="@/assets/gladiator-studios.png" media="(max-width: 768px)">
        <img class="page active" src="@/assets/originals/gladiator-studios.png">
      </picture>
      <picture>
        <source srcset="@/assets/my-gold-animals.png" media="(max-width: 768px)">
        <img class="page active" src="@/assets/originals/my-gold-animals.png">
      </picture>
    </div>
    <div class="project-list-navigation">
      <div class="project-list-wrapper">
        <!---->
        <div class="project-list-window">
          <ul id="projectListBottom" class="project-list list-unstyled list-inline" style="left: 0px;">
            <li v-bind:class="{active: active1}" v-on:click="makeActive1">
              <div class="icon" :style="{ backgroundImage: 'url(' + require('@/assets/pw-quickmenu-icon.png') + ')' }"></div> <span>Personal Website</span>
            </li>
            <li v-bind:class="{active: active2}" v-on:click="makeActive2">
              <div class="icon" :style="{ backgroundImage: 'url(' + require('@/assets/lyf-quickmenu-icon.png') + ')' }"></div> <span>LoveYouForever</span>
            </li>
            <li v-bind:class="{active: active3}" v-on:click="makeActive3">
              <div class="icon" :style="{ backgroundImage: 'url(' + require('@/assets/bikev1-quickmenu-icon.png') + ')' }"></div> <span>Bike Finder</span>
            </li>
            <li v-bind:class="{active: active4}" v-on:click="makeActive4">
              <div class="icon" :style="{ backgroundImage: 'url(' + require('@/assets/bikev2-quickmenu-icon.png') + ')' }"></div> <span>Bike Finder 2</span>
            </li>
            <li v-bind:class="{active: active5}" v-on:click="makeActive5">
              <div class="icon" :style="{ backgroundImage: 'url(' + require('@/assets/gs-quickmenu-icon.png') + ')' }"></div> <span>Gladiator Studios</span>
            </li>
            <li v-bind:class="{active: active6}" v-on:click="makeActive6">
              <div class="icon" :style="{ backgroundImage: 'url(' + require('@/assets/mga-quickmenu-icon.png') + ')' }"></div> <span>My Gold Animals</span>
            </li>
          </ul>
        </div>

      </div>
      <div class="all-projects">
        <div class="icon"><a class="">
            <svg data-v-6c07c8b2="" id="icon-all-project" viewBox="0 0 36 36" width="100%" height="100%">
              <path data-v-6c07c8b2="" d="M7.72,6h5.14a1.72,1.72,0,0,1,1.72,1.71v5.15a1.72,1.72,0,0,1-1.72,1.71H7.72A1.71,1.71,0,0,1,6,12.89V7.74A1.71,1.71,0,0,1,7.72,6Z" transform="translate(-6.01 -6.03)" class="white"></path>
              <path data-v-6c07c8b2="" d="M21.43,6h5.15a1.72,1.72,0,0,1,1.71,1.71v5.15a1.72,1.72,0,0,1-1.71,1.71H21.43a1.72,1.72,0,0,1-1.71-1.71V7.74A1.72,1.72,0,0,1,21.43,6Z" transform="translate(-6.01 -6.03)" class="white"></path>
              <path data-v-6c07c8b2="" d="M35.15,6h5.14A1.72,1.72,0,0,1,42,7.74v5.15a1.72,1.72,0,0,1-1.72,1.71H35.15a1.72,1.72,0,0,1-1.72-1.71V7.74A1.72,1.72,0,0,1,35.15,6Z" transform="translate(-6.01 -6.03)" class="white"></path>
              <path data-v-6c07c8b2="" d="M7.72,19.74h5.14a1.72,1.72,0,0,1,1.72,1.72V26.6a1.71,1.71,0,0,1-1.72,1.71H7.72A1.7,1.7,0,0,1,6,26.6V21.46A1.71,1.71,0,0,1,7.72,19.74Z" transform="translate(-6.01 -6.03)" class="white"></path>
              <path data-v-6c07c8b2="" d="M21.43,19.74h5.15a1.72,1.72,0,0,1,1.71,1.72V26.6a1.71,1.71,0,0,1-1.71,1.71H21.43a1.71,1.71,0,0,1-1.71-1.71V21.46A1.72,1.72,0,0,1,21.43,19.74Z" transform="translate(-6.01 -6.03)" class="white"></path>
              <path data-v-6c07c8b2="" d="M35.15,19.74h5.14A1.72,1.72,0,0,1,42,21.46V26.6a1.71,1.71,0,0,1-1.72,1.71H35.15a1.71,1.71,0,0,1-1.72-1.71V21.46A1.72,1.72,0,0,1,35.15,19.74Z" transform="translate(-6.01 -6.03)" class="white"></path>
              <path data-v-6c07c8b2="" d="M7.72,33.46h5.14a1.71,1.71,0,0,1,1.72,1.71v5.14A1.72,1.72,0,0,1,12.86,42H7.72A1.71,1.71,0,0,1,6,40.31V35.17A1.7,1.7,0,0,1,7.72,33.46Z" transform="translate(-6.01 -6.03)" class="white"></path>
              <path data-v-6c07c8b2="" d="M21.43,33.46h5.15a1.71,1.71,0,0,1,1.71,1.71v5.14A1.72,1.72,0,0,1,26.58,42H21.43a1.72,1.72,0,0,1-1.71-1.72V35.17A1.71,1.71,0,0,1,21.43,33.46Z" transform="translate(-6.01 -6.03)" class="white"></path>
              <path data-v-6c07c8b2="" d="M35.15,33.46h5.14A1.71,1.71,0,0,1,42,35.17v5.14A1.72,1.72,0,0,1,40.29,42H35.15a1.72,1.72,0,0,1-1.72-1.72V35.17A1.71,1.71,0,0,1,35.15,33.46Z" transform="translate(-6.01 -6.03)" class="white"></path>
            </svg>
            All Projects
          </a></div>
      </div>

      <div class="clearfix"></div>
    </div>

  </div>
</template>

<script>
export default {
  data(){
    return{
      active1: true,
      active2: false,
      active3: false,
      active4: false,
      active5: false,
      active6: false
    }
  },
  methods: {
    makeActive1(){
      this.active1 = true;
      this.active2 = false;
      this.active3 = false;
      this.active4 = false;
      this.active5 = false;
      this.active6 = false;
    },
    makeActive2(){
      this.active2 = true;
      this.active1 = false;
      this.active3 = false;
      this.active4 = false;
      this.active5 = false;
      this.active6 = false;
    },
    makeActive3(){
      this.active3 = true;
      this.active2 = false;
      this.active1 = false;
      this.active4 = false;
      this.active5 = false;
      this.active6 = false;
    },
    makeActive4(){
      this.active4 = true;
      this.active2 = false;
      this.active3 = false;
      this.active1 = false;
      this.active5 = false;
      this.active6 = false;
    },
    makeActive5(){
      this.active5 = true;
      this.active2 = false;
      this.active3 = false;
      this.active4 = false;
      this.active1 = false;
      this.active6 = false;
    },
    makeActive6(){
      this.active6 = true;
      this.active2 = false;
      this.active3 = false;
      this.active4 = false;
      this.active5 = false;
      this.active6 = false;
    }
  }
}
</script>


<style lang="scss" scoped>
.wrapper {
  .card-project {
    background: #2e3138;
    box-shadow: 0 0 15px 1px rgba(0, 0, 0, 0.7);
    border: 1px solid #383b42;
    opacity: 1;
    color: #c6d4df;
    .capsule {
      a {
        text-decoration: none;
        .thumb {
          height: 177px;
        }
      }

      .wrapper {
        .description {
          font-family: "Motiva Sans", Sans-serif;
          font-weight: 300;
          font-size: 15px;
          justify-self: flex-start;
        }
        .block-skills {
          min-height: 18px;
          line-height: 15px;
          color: #acdbf5;
        }
      }
    }
  }
}
.links {
  max-height: 40px;
  align-self: flex-end;
}
#projects {
  background: #2e3138;
}
.container {
  background: url("../assets/personal-website.png");
  width: 100%;
  height: 700px;
  opacity: 0.7;
  background-repeat: no-repeat;
}
.project-list-navigation {
  background-color: #1a1a1a;
  position: fixed;
  bottom: 0px;
  transition: 0.2s;
  height: 100px;
  width: 100%;
}
.project-list-navigation .select-project-type {
  padding-left: 60px;
  margin-top: 15px;
  position: absolute;
  left: 0;
}
.project-list-navigation .project-list-wrapper {
  width: 720px;
  padding: 0 40px;
  position: relative;
  height: 100px;
  margin: 0 auto;
}
.project-list-navigation .all-projects {
  position: absolute;
  right: 0;
  top: 0;
  cursor: pointer;
}
.project-list-navigation .project-list-wrapper .project-list-window {
  width: 810px;
  height: 100px;
  overflow: hidden;
  position: absolute;
}
.project-list-navigation .icon-next {
  right: 0;
}
.project-list-navigation .project-list-wrapper .project-list {
  position: absolute;
  white-space: nowrap;
  left: 0;
  transition: left 0.5s;
}
.project-list-navigation .project-list-wrapper .project-list li.active {
  color: #fff;
  background-color: #121212;
}
.project-list-navigation .project-list-wrapper .project-list li {
  display: inline-block;
  width: 128px;
  cursor: pointer;
  color: hsla(0, 0%, 100%, 0.4);
  vertical-align: top;
  height: 100px;
  transition: color 0.3s;
}
.list-inline > li {
  display: inline-block;
  padding-left: 5px;
  padding-right: 5px;
}
.project-list-navigation .project-list-wrapper .project-list li {
  display: inline-block;
  width: 128px;
  cursor: pointer;
  color: hsla(0, 0%, 100%, 0.4);
  vertical-align: top;
  height: 100px;
  transition: color 0.3s;
}
.list-inline > li {
  display: inline-block;
  padding-left: 5px;
  padding-right: 5px;
}
.project-list-navigation .project-list-wrapper .project-list .icon {
  background-repeat: no-repeat;
  // width: 44px;
  height: 44px;
  margin: 0 auto;
  margin-top: 15px;
  opacity: 0.3;
}

.project-list-navigation .project-list-wrapper .project-list li span {
  white-space: pre-wrap;
  display: block;
  margin-top: 7px;
  font-size: 12px;
  line-height: 1.2em;
  height: 28px;
  text-align: center;
}
.project-list-navigation .project-list-wrapper .project-list li.active .icon {
  opacity: 1;
}
.project-list-navigation .project-list-wrapper .project-list li {
  display: inline-block;
  width: 128px;
  cursor: pointer;
  color: hsla(0, 0%, 100%, 0.4);
  vertical-align: top;
  height: 100px;
  transition: color 0.3s;
}
.project-list-navigation .project-list-wrapper .project-list {
  position: absolute;
  white-space: nowrap;
  left: 0;
  transition: left 0.5s;
}
.list-inline {
  margin-left: -5px;
}
.list-inline,
.list-unstyled {
  padding-left: 0;
  list-style: none;
}
ol,
ul {
  margin-top: 0;
  margin-bottom: 7px;
  line-height: 1.5em;
}
body {
  overflow-y: hidden;
}
.icon {
  background-position-x: center;
}
.project-list-navigation .all-projects {
  position: absolute;
  right: 0;
  top: 0;
  cursor: pointer;
}
.project-list-navigation .all-projects .icon {
  display: inline-block;
  width: 160px;
  text-align: center;
}
.project-list-navigation .all-projects a {
  display: inline-block;
  margin-top: 30px;
  color: #fff;
  opacity: 0.5;
  transition: opacity 0.3s;
}
a,
a:focus,
a:hover {
  text-decoration: none;
}
.project-list-navigation .all-projects a #icon-all-project {
  width: 21px;
  height: 21px;
  display: block;
  margin: 0 auto 10px;
}
svg:not(:root) {
  overflow: hidden;
}
.project-list-navigation .all-projects a {
  display: inline-block;
  margin-top: 30px;
  color: #fff;
  opacity: 0.5;
  transition: opacity 0.3s;
}
.white {
  fill: white;
}
.project-list-navigation .project-list-wrapper .project-list li span {
  white-space: pre-wrap;
  display: block;
  margin-top: 7px;
  font-size: 12px;
  line-height: 1.2em;
  height: 28px;
  text-align: center;
  font-family: Arial, sans-serif;
  font-size: 14px;
  line-height: 1;
  color: #737373;
}
.project-list-navigation .project-list-wrapper .project-list li.active span {
  color: white;
}
.scroll-container {
  width: 100%;
  height: 100%;
}
@media (max-height: 980px) {
  .fullpage-container {
    height: 100% !important;
    top: 0;
  }
}
.fullpage-container {
  position: absolute;
  left: 0;
  width: 100%;
}
.fullpage-container {
  position: relative;
  height: 100%;
  overflow: hidden;
}
.fullpage-container .fullpage-wp.anim {
  transition: 0.2s;
}
.fullpage-wp.anim {
  transform: translateZ(0);
  transition: all 0.5s ease-out 0s;
}
.animated {
  opacity: 1;
}
.fullpage-wp {
}
.fadeIn {
  animation-name: fadeIn;
}

.animated {
  animation-duration: 1s;
  animation-fill-mode: both;
}
.page.active {
  opacity: 1;
  transition: all 1s;
}
.page {
  background: transparent no-repeat center;
  background-size: cover;
  position: relative;
  width: 100%;
  height: 100%;
  opacity: 0.3;
}
.page {
  box-sizing: border-box;
  display: block;
  -ms-flex-negative: 0;
  flex-shrink: 0;
  overflow: hidden;
}
@media (max-height: 980px) {
  .fullpage-container .page .project-information {
    padding-top: 80px;
  }
}
.project-information,
.launcher-information {
  position: relative;
  padding-top: 10px;
  padding-left: 60px;
}
.project-information .logo,
.launcher-information .logo {
  height: 18vh;
  display: table-cell;
  vertical-align: middle;
}
a,
a:focus,
a:hover {
  text-decoration: none;
}
a {
  color: #737373;
}
a {
  background-color: transparent;
}
.project-information .logo > div,
.launcher-information .logo > div {
  display: inline-block;
  background-size: contain;
  background-repeat: no-repeat;
  background-position: left 50%;
  width: 420px;
  height: 18vh;
}
.project-information .project-info,
.launcher-information .project-info {
  color: #adadad;
  font-size: 14px;
  text-shadow: 0 0 1px rgba(0, 0, 0, 0.5);
}
.list-inline {
  margin-left: -5px;
}
.list-inline,
.list-unstyled {
  padding-left: 0;
  list-style: none;
}
ol,
ul {
  margin-top: 0;
  margin-bottom: 7px;
  line-height: 1.5em;
}
.project-information .project-desc,
.launcher-information .project-desc {
  color: hsla(0, 0%, 100%, 0.75);
  text-shadow: 0 0 1px rgba(0, 0, 0, 0.85);
  font-size: 16px;
  width: 550px;
}
p {
  margin: 0 0 7px;
  line-height: 1.5em;
}
.project-information .learn-more,
.launcher-information .learn-more {
  font-size: 12px;
  font-weight: 700;
  text-transform: uppercase;
  color: hsla(0, 0%, 100%, 0.85);
  text-shadow: 0 0 1px rgba(0, 0, 0, 0.85);
  margin-top: 30px;
  display: inline-block;
}
a,
a:focus,
a:hover {
  text-decoration: none;
}
a {
  color: #737373;
}

a {
  background-color: transparent;
}
.list-inline > li {
  display: inline-block;
  padding-left: 5px;
  padding-right: 5px;
}
p {
  margin: 0 0 7px;
  line-height: 1.5em;
}
.project-information .project-info,
.launcher-information .project-info {
  color: #adadad;
  font-size: 14px;
  text-shadow: 0 0 1px rgba(0, 0, 0, 0.5);
}
.project-information .project-info span,
.launcher-information .project-info span {
  color: #fff;
  margin-left: 5px;
}

p {
  color: hsla(0, 0%, 100%, 0.75);
  text-shadow: 0 0 1px rgba(0, 0, 0, 0.85);
  font-size: 16px;
  width: 550px;
}
@media (max-width: 1024px) {
  .fullpage-container .fullpage-wp {
    transform: none !important;
  }
}

@media (max-width: 480px) {
  .page {
    // height: 250px !important;
  }
}
@media (max-width: 768px) {
  .page {
  }
}
@media (max-width: 1024px) {
  .page {
    top: 0;
    opacity: 1;
  }
}
@media (max-height: 980px) {
  .fullpage-container .page .project-information {
    padding-top: 80px;
  }
}
@media (max-width: 768px) {
  .page .project-information {
    padding-top: 0 !important;
  }
  .fullpage-wp {
    margin-top: 35px;
    margin-bottom: 35px;
  }
  .project-list-navigation {
    display: none;
  }
}
@media (max-width: 1024px) {
  .page .project-information {
    text-align: center;
    padding-left: 0;
  }
}
@media (max-width: 480px) {
  .page .project-information .logo {
    height: auto;
    display: block;
    padding: 0;
  }
}
@media (max-width: 1024px) {
  .page .project-information .logo {
  }
}
#projects > div.fullpage-container > div > div {
  background-size: contain;
}
@media (max-width: 425px) {
  .project-list-navigation {
    display: none;
  }
  .page {
    background-size: contain;
    height: 332px !important;
  }
}

@media (max-width: 320px) {
  .page {
    background-size: contain;
    height: 250px !important;
  }
}
</style>
