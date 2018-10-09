<template>
  <div id="projects">

    <div class="card-project">
      <div class="capsule">
        <div class="wrapper">
          <a href="/">
          <img class="thumb" src="@/assets/portfolio-website.png" alt="" srcset="" width="358px"  height="177px">
          </a>
          <div class="block">
            Vue - Flexbox - Webpack - SCSS - TypeScript
          </div>
        <div class="description">
          <p>I created this website from scratch.</p>
        </div></div>
        
        
      </div>
    </div>
    <div class="card-project">
      <div class="capsule">
        <div class="wrapper">
          <a href="https://github.com/eugenefedoto/LoveYouForever">
          <img class="thumb" src="@/assets/love-you-forever.png" alt="" srcset="" width="376px" height="177px">
          </a>
          <div class="block">
            Vue - CSS Grid - Laravel - Docker - Apache
          </div>
        <div class="description">
          <p>A creative playground for myself - based on the hit game and anime Amagami SS. It started out as a challenge to learn CSS Grid Layout and Docker. Soon it transformed into a playground, allowing me to test out new features and frameworks on a whim.</p>
        </div>
        </div>
        
        
      </div>
    </div>
    <div class="card-project">
      <div class="capsule">
        <div class="wrapper"><a href="">
          <img class="thumb" src="@/assets/bike-location-finder-v1.png" alt="" srcset="" width="373px" height="177px">
          </a>
          <div class="block">
            Vue - Semantic UI - Node.js - MongoDB
          </div>
        <div class="description">
          <p>A project I lead across two teams for the https://fullstack.network/ contest. It won first place for fastest completion, organization and management categories. I designed the entire UI myself, and initially developed the entire backend and database myself; before transferring the backend to a new team. 400k+ data points.</p>
        </div></div>
        
        
      </div>
    </div>
    <div class="card-project">
      <div class="capsule">
        <div class="wrapper"><a href="">
          <img class="thumb" src="@/assets/bike-location-finder-v2.png" alt="" srcset="" width="373px" height="177px">
          </a>
          <div class="block">
            Vue - Vuetify - Go - SQLite - Mapillary
          </div>
        <div class="description">
          <p>Version 2 of the Bike Network Location Finder. I redesigned the entire UI to have cleaner code, be modular, and use the Vuetify library.</p>
        </div></div>
        
        
      </div>
    </div>
    <div class="card-project">
      <div class="capsule">
        <div class="wrapper"><a href="">
          <img class="thumb" src="@/assets/gladiator-studios.png" alt="" srcset="" width="376px" height="177px">
          </a>
          <div class="block">
            HTML - CSS - JavaScript - Adobe Photoshop
          </div>
        <div class="description">
          <p>A portfolio website, involving Gladiator jewelry that I developed for a jeweler. It consisted of slicing PSD files, photoshopping some custom effects, and adding sliders.</p>
        </div></div>
        
        
      </div>
    </div>
    <div class="card-project">
      <div class="capsule">
        <div class="wrapper"><a href="">
          <img class="thumb" src="@/assets/my-gold-animals.png" alt="" srcset="" width="376px" height="177px">
          </a>
          <div class="block">
            HTML - CSS - JavaScript - Adobe Photoshop - PrestaShop
          </div>
        <div class="description">
          <p>A portfolio website, involving pet jewelry that I developed for a jeweler. It involved similar design work to that of the Gladiator Studios project. This time I added the PrestaShop framework to improve efficiency of adding pages and managing a store. I added some custom PHP code for my needs.</p>
        </div></div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
#projects {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  .card-project {
    background: #2e3138;
    box-shadow: 0 0 15px 1px rgba(0, 0, 0, 0.7);
    border: 1px solid #383b42;
    padding: 15px;
    width: 400px;
    opacity: 1;
    height: 348px;
    color: #c6d4df;
    margin: 20px 10px;
    .capsule {
      // display:flex;
      a {
        text-decoration: none;
        display: flex;
        flex-direction: column;
        align-items: center;
        .thumb {
          height: 177px;
        }
      }
      .block {
          min-height: 18px;
          line-height: 15px;
          color: #acdbf5;
        }
      .description {
        font-family: "Motiva Sans", Sans-serif;
        font-weight: 300;
        font-size: 15px;
        align-self: flex-start;
        .details {
          margin-top: -19px;
          height: 23px;
        }
      }
      .wrapper {
        display: flex;
        flex-direction: column;
        align-items: center;
      }
    }
  }
}
</style>

