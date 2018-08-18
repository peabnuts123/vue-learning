<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    
    <div class="Container">
      <div class="router-view-wrapper">
        <div class="router-view">
          <router-view />
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
  @import "./styles/app.scss";

  .router-view-wrapper {
    position: relative;
  }

  // Target the view itself
  .router-view>* {
    position: absolute;
    width: 100%;
    text-align: center;
  }

  .Container {
    max-width: 1024px;
    margin-left: auto;
    margin-right: auto;
  }

  #app {
    font-family: "Avenir", Helvetica, Arial, sans-serif;
    color: #2c3e50;
    text-align: center;
    // Better Font Rendering
    font-feature-settings: "kern" 1;
    font-kerning: normal;
    text-rendering: optimizeLegibility;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
  }
  #nav {
    padding: 30px;
    a {
      font-weight: bold;
      color: #2c3e50;
      &.router-link-exact-active {
        color: #42b983;
      }
    }
  }
</style>
