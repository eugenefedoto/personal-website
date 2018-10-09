<template>
  <div id="projects">

    <div id="personal-website" class="card-project">
      <div class="capsule">
        <div class="wrapper">
          <a href="/">
          <img class="thumb" src="@/assets/personal-website.png" alt="" srcset="" width="358px"  height="177px">
          </a>
          <div class="block-skills">
            Vue - Flexbox - Webpack - SCSS - TypeScript
          </div>
        <div class="description">
          <p>My person website created from scratch.</p>
        </div>
        </div>
      </div>
      <div class="links">
          <a target="_blank" href="https://github.com/eugenefedoto/eugenefedoto.github.io"><img src="@/assets/Octocat.png" alt="" width="40" height="33"></a>
        </div>
    </div>
    <div id="love-you-forever" class="card-project">
      <div class="capsule">
        <div class="wrapper">
          <img class="thumb" src="@/assets/love-you-forever.png" alt="" srcset="" width="376px" height="177px">
          <div class="block-skills">
            Vue - CSS Grid - Laravel - Docker - Apache
          </div>
        <div class="description">
          <p>A creative playground for developing my skills - based on the hit game and anime Amagami SS.</p>
        </div>

        </div>
      </div>
      <div class="links">
          <a target="_blank" href="https://github.com/eugenefedoto/LoveYouForever"><img src="@/assets/Octocat.png" alt="" width="40" height="33"></a>
        </div>
    </div>
    <div id="bike-location-finder-v1" class="card-project">
      <div class="capsule">
        <div class="wrapper"><a href="https://seagulltuna.neuralspaz.com/">
          <img class="thumb" src="@/assets/bike-location-finder-v1.png" alt="" srcset="" width="373px" height="177px">
          </a>
          <div class="block-skills">
            Vue - Semantic UI - Node.js - MongoDB
          </div>
        <div class="description">
          <p>Google Maps for bikes, with over 400k interactive points. A first place, team project for the https://fullstack.network/ contest.</p>
        </div></div>
      </div>
      <div class="links">
          <a target="_blank" href="https://github.com/getbikesharedone/seagulltuna"><img src="@/assets/Octocat.png" alt="" width="40" height="33"></a>
        </div>
    </div>
    <div id="bike-location-finder-v2" class="card-project">
      <div class="capsule">
        <div class="wrapper"><a href="https://seagulltunav2.neuralspaz.com/">
          <img class="thumb" src="@/assets/bike-location-finder-v2.png" alt="" srcset="" width="373px" height="177px">
          </a>
          <div class="block-skills">
            Vue - Vuetify - Go - SQLite - Mapillary
          </div>
        <div class="description">
          <p>Version 2 of the Bike Network Location Finder. I redesigned the entire UI to have cleaner code, be modular, and use the Vuetify library.</p>
        </div></div>
      </div>
      <div class="links">
          <a target="_blank" href="https://github.com/getbikesharedone/seagulltunav2"><img src="@/assets/Octocat.png" alt="" width="40" height="33"></a>
        </div>
    </div>
    <div id="gladiator-studios" class="card-project">
      <div class="capsule">
        <div class="wrapper"><a href="http://www.gladiator-studios.com/">
          <img class="thumb" src="@/assets/gladiator-studios.png" alt="" srcset="" width="376px" height="177px">
          </a>
          <div class="block-skills">
            HTML - CSS - JavaScript - Adobe Photoshop
          </div>
        <div class="description">
          <p>A portfolio website, involving Gladiator jewelry, that I created for a jeweler.</p>
        </div></div>
      </div>
    </div>

<div id="my-gold-animals" class="card-project">
      <div class="capsule">
        <div class="wrapper"><a href="http://mygoldanimals.com/">
          <img class="thumb" src="@/assets/my-gold-animals.png" alt="" srcset="" width="376px" height="177px">
          </a>
          <div class="block-skills">
            HTML - CSS - JavaScript - Adobe Photoshop - PrestaShop
          </div>
        <div class="description">
          <p>Another portfolio website, but this time for pet jewelry that I created for a jeweler. This time an ecommerce backend was added.</p>
        </div></div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
#projects {
  display: flex;
  justify-content: space-evenly;
  flex-wrap: wrap;
  .card-project {
    background: #2e3138;
    box-shadow: 0 0 15px 1px rgba(0, 0, 0, 0.7);
    border: 1px solid #383b42;
    opacity: 1;
    color: #c6d4df;
    margin: 20px 10px;
    display:flex;
    flex-wrap: wrap;
    .capsule {
      a {
        text-decoration: none;
        .thumb {
          height: 177px;
        }
      }

      .wrapper {
        display: flex;
        flex-wrap: wrap;
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
  #personal-website {
    max-width: 358px;
  }
  #love-you-forever,
  #gladiator-studios,
  #my-gold-animals {
    max-width: 376px;
  }
  #bike-location-finder-v1,
  #bike-location-finder-v2 {
    max-width: 373px;
  }
}
.links {
  max-height: 40px;
  align-self: flex-end;
  
}
</style>

