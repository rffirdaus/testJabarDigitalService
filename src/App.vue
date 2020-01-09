<template>
  <div id="app">
    <div id="nav" class="d-flex justify-content-center">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <router-view />
  </div>
</template>

<style lang="scss">
@import "./src/styles/global.scss";
</style>
