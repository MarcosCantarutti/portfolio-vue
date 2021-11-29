<template>
  <div id="nav">
    <div class="menu">
      <router-link to="/">Home</router-link> 
      <router-link to="/projects">Projetos</router-link>
      <router-link to="/contacts">Contato</router-link>
    </div>
    
  </div>
  <router-view/>
</template>

<style lang="scss">
$background: #181818;
$background-routers: #212121;

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  font-size: 62.5%;
}

body {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background: $background;
  
}

#app {
  display: flex;
}


#nav {
  
  max-width: 30rem;
  height: 100vh;
  background: $background-routers;
  display: flex;
  padding: 5rem;
  margin-right: 3rem;
  -webkit-box-shadow: inset -1px 3px 8px 5px #554BFF, 2px 5px 16px 0px #554BFF, 1px 1px 1px 1px #554BFF; 
  box-shadow: inset -1px 3px 8px 5px #554BFF, 2px 5px 16px 0px #554BFF, 1px 1px 1px 1px #554BFF;
 
 
  a {
    text-decoration: none;
    font-size: 2rem;
    font-weight: bold;
    color: #FEFBFB;

    &.router-link-exact-active {
      color: #554BFF;
    }
  }

  .menu {
     display: flex;
    flex-direction: column;
    padding: 3rem;
    gap: 2rem;
    width: 100%;

    align-items: center;
    justify-content: center;
    
  }
}
</style>
