<template>
  <div id="app">
    <!--<div id="nav">-->
      <!--<router-link to="/">Home</router-link> |-->
      <!--<router-link to="/about">About</router-link>-->
    <!--</div>-->
    <router-view/>
  </div>
</template>

<style lang="scss">
  *{
    margin: 0;
    padding: 0;
    text-decoration: none;
    font-size: 1.4rem;
  }
  html{
    font-size: 10px;
      width: 100vw;
      overflow-x: hidden;
  }
</style>
