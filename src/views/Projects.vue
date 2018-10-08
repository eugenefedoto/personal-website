<template>
  <div id="projects">
    <div class="container-thumbs">
      <div class="wrapper-project"><img id="thm1" src="@/assets/love-you-forever.png" alt="" srcset=""></div>
      <div class="wrapper-project"><img id="thm2" src="@/assets/bike-location-finder-v2.png" alt="" srcset=""></div>
      <div class="wrapper-project"><img id="thm3" src="@/assets/bike-location-finder-v1.png" alt="" srcset=""></div>
      <div class="wrapper-project"><img id="thm4" src="@/assets/gladiator-studios.png" alt="" srcset=""></div>
      <div class="wrapper-project"><img id="thm5" src="@/assets/my-gold-animals.png" alt="" srcset=""></div>
      <div class="wrapper-project"><img id="thm6" src="@/assets/table-parking.png" alt="" srcset=""></div>
    </div>
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
      &#thm1, &#thm4{
        width:100%;
      }
      &#thm2, &#thm3, &#thm5, &#thm6{
        width:700px;
      }
    }
  }
}
</style>

