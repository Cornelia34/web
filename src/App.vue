<template>
  <div id="app">
    <div id="topContainer">
      <div id="nav">
        <router-link to="/">Home</router-link> |
        <router-link to="/about">About</router-link> |
        <router-link to="/news">News</router-link> |
        <router-link to="/activity">Activity</router-link> |
        <router-link to="/contect">Contect</router-link>
      </div>
      <router-view/>
    </div>
  </div>
</template>

<style>
#app {
  font-family: Verdana;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #5A5757;
  letter-spacing: 2px
}

#nav {
  padding: 15px;
}

#nav a {
  text-decoration: none;
  font-weight: bold;
  color:  #5A5757;
}

#nav a.router-link-exact-active {
  color: #AAB8BB;
}

</style>
