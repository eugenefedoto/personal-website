<template>
  <div id="app">
    <router-view/>
    <div class="overlay">
        <div class="wrapper">
            <router-link to="/" id="logo">ef_</router-link>
            <nav class="tabs">
                <div class="selector"></div>
                <router-link to="/projects" class="uppercase">projects</router-link>
                <router-link to="/hacking" class="uppercase">misc</router-link>
            </nav>
        </div>
        <div class="desc">Eugene Fedotov</div>
        <div class="desc">is a <span class="uppercase subject">hacker</span></div>
        <div class="desc">is a <span class="uppercase subject">developer</span></div>
        <div class="desc">loves <span class="uppercase subject">anime</span></div>
    </div>
  </div>
</template>

<style lang="scss">
@import "~normalize.css";
.overlay {
  position: absolute;
  font-family: Nobile, sans-serif;
  font-size: 2rem;
  margin-top: 10px;
  margin-left: 50px;
  .desc {
    font-size: 2em;
    color: white;
    .uppercase {
      text-transform: uppercase;
    }
  }
  .wrapper {
    display: flex;
    margin-top: 1rem;
    margin-bottom: 2rem;
    #logo {
      margin: 0 1.5rem;
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
        &:hover{
          color: #ff006a;
        }
      }
    }
  }
  .subject,
  #logo {
    text-decoration: none;
    background: linear-gradient(to right, #30cfd0 0%, #6410cc 100%);
    background-clip: text;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
}
</style>
