<template>
  <div id="app">
    <div id="nav">
      <router-link :to="{name:'home'}">home</router-link>
      <router-link :to="{name:'about'}">about</router-link>
    </div>
    <router-view />
    <router-view name="email" />
    <router-view name="tel" />
  </div>
</template>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  padding: 30px;
  a {
    padding-right: 20px;
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
