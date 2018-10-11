<template>
  <div id="app">
    <div class="wrapper-nav">
        <router-link to="/" id="logo">ef_</router-link>
        <nav class="tabs">
            <div class="selector"></div>
            <router-link to="/projects" class="uppercase">projects</router-link>
        </nav>
    </div>
    <router-view/>
  </div>
</template>

<style lang="scss">
@import "~normalize.css";
body {
  background: #2e3138;
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
  #logo {
    text-decoration: none;
    background: linear-gradient(to right, #30cfd0 0%, #6410cc 100%);
    background-clip: text;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
  .desc {
    font-size: 2em;
    color: white;
    .subject{
      font-size: 0.6em;
    }
  }
}
.uppercase {
      text-transform: uppercase;
    }
</style>
