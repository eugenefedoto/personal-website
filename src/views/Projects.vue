<template>
  <div id="projects">

    <div class="card-project">
      <div class="capsule">
        <a href="">
          <img class="thumb" src="@/assets/portfolio-website.png" alt="" srcset="">
          <div class="block">
            Vue - Flexbox - Webpack - SCSS - TypeScript
          </div>
          </a>
        <div class="description">
 
          <p>My portfolio website was created from scratch. I focused on showcasing my personality, and writing great code.</p>
        </div>
        
      </div>
    </div>
    <div class="card-project">
      <div class="capsule">
        <a href="">
          <img class="thumb" src="@/assets/love-you-forever.png" alt="" srcset="">
          <div class="block">
            Vue - CSS Grid - Laravel - Docker - Apache
          </div>
          </a>
        <div class="description">
 
          <p>A creative playground for myself - based on the hit game and anime Amagami SS. It started out as a challenge to learn CSS Grid Layout and Docker. Soon it transformed into a playground, allowing me to test out new features and frameworks on a whim.</p>
        </div>
        
      </div>
    </div>
    <div class="card-project">
      <div class="capsule">
        <a href="">
          <img class="thumb" src="@/assets/bike-location-finder-v1.png" alt="" srcset="">
          <div class="block">
            Vue - Semantic UI - Node.js - MongoDB
          </div>
          </a>
        <div class="description">

          <p>A project I lead across two teams for the https://fullstack.network/ contest. It won first place for fastest completion, organization and management categories. I designed the entire UI myself, and initially developed the entire backend and database myself; before transferring the backend to a new team. 400k+ data points.</p>
        </div>
        
      </div>
    </div>
    <div class="card-project">
      <div class="capsule">
        <a href="">
          <img class="thumb" src="@/assets/bike-location-finder-v2.png" alt="" srcset="">
          <div class="block">
            Vue - Vuetify - Go - SQLite - Mapillary
          </div>
          </a>
        <div class="description">
          <p>Version 2 of the Bike Network Location Finder. I redesigned the entire UI to have cleaner code, be modular, and use the Vuetify library.</p>
        </div>
        
      </div>
    </div>
    <div class="card-project">
      <div class="capsule">
        <a href="">
          <img class="thumb" src="@/assets/gladiator-studios.png" alt="" srcset="">
          <div class="block">
            HTML - CSS - JavaScript - Adobe Photoshop
          </div>
          </a>
        <div class="description">
          <p>A portfolio website, involving Gladiator jewelry that I developed for a jeweler. It consisted of slicing PSD files, photoshopping some custom effects, and adding sliders.</p>
        </div>
        
      </div>
    </div>
    <div class="card-project">
      <div class="capsule">
        <a href="">
          <img class="thumb" src="@/assets/my-gold-animals.png" alt="" srcset="">
          <div class="block">
            HTML - CSS - JavaScript - PHP - Adobe Photoshop - PrestaShop - MySQL
          </div>
          </a>
        <div class="description">
          <p>A portfolio website, involving pet jewelry that I developed for a jeweler. It involved similar design work to that of the Gladiator Studios project. This time I added the PrestaShop framework to improve efficiency of adding pages and managing a store. I added some custom PHP code for my needs.</p>
        </div>
        
      </div>
    </div>
    
    <!-- <div class="container-thumbs">
      <div class="wrapper-project"><img id="thm1" src="@/assets/love-you-forever.png" alt="" srcset=""></div>
      <div class="wrapper-project"><img id="thm2" src="@/assets/bike-location-finder-v2.png" alt="" srcset=""></div>
      <div class="wrapper-project"><img id="thm3" src="@/assets/bike-location-finder-v1.png" alt="" srcset=""></div>
      <div class="wrapper-project"><img id="thm4" src="@/assets/gladiator-studios.png" alt="" srcset=""></div>
      <div class="wrapper-project"><img id="thm5" src="@/assets/my-gold-animals.png" alt="" srcset=""></div>
      <div class="wrapper-project"><img id="thm6" src="@/assets/table-parking.png" alt="" srcset=""></div>
    </div> -->
  </div>
</template>

<style lang="scss" scoped>
.container-thumbs {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  margin-top: 5vh;
  .wrapper-project {
    margin: 1vh 1vw;
    img {
      &#thm1,
      &#thm4 {
        width: 100%;
      }
      &#thm2,
      &#thm3,
      &#thm5,
      &#thm6 {
        width: 700px;
      }
    }
  }
}
#projects{
  width:940px;
  margin:0 auto;
  display:flex;
  flex-wrap: wrap;
}
.card-project {
  background: #2e3138;
  box-shadow: 0 0 15px 1px rgba(0, 0, 0, 0.7);
  border:1px solid #383b42;
  padding:15px;
  width: 40%;
  display: flex;
  opacity: 1;
  height: 348px;
  color: #c6d4df;
  margin: 20px 10px;
  .capsule {
    flex-shrink: 5;
    flex-basis: 100%;
    
    a {
      text-decoration:none;
      .thumb {
        width: 100%;
        max-height: 177px;
      }
      .block{
        min-height: 18px;
        line-height: 15px;
        color:#acdbf5
      }
    }
    .description {
          font-family: "Motiva Sans", Sans-serif;
    font-weight: 300;
    font-size: 15px;

      .details {
        margin-top: -19px;
        height: 23px;
      }
    }
  }
  .contents {
    flex-shrink: 3.1;
    flex-basis: 100%;
    max-height: 100%;
    margin-left: 15px;
    background: rgba(0, 0, 0, 0.1);
  }
}
.screenshots {
  div {
    width: 50%;
    height: 50%;
    background-size: cover;
    overflow: hidden;
    background-repeat: no-repeat;
    box-shadow: 0 0 1px #000 inset;
  }
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  height: 100%;
}
</style>

