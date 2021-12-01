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

@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap');

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
  font-family: 'Poppins', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background: $background;
  overflow-x: hidden;
  overflow-y: hidden;
  
}

h1, h2, h3 {
  font-weight: 700;
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
  
  -webkit-box-shadow: inset -1px 3px 8px 5px #554BFF, 2px 5px 16px 0px #554BFF, 1px 1px 1px 1px #554BFF; 
  box-shadow: inset -1px 3px 8px 5px #554BFF, 2px 5px 16px 0px #554BFF, 1px 1px 1px 1px #554BFF;
 
  a {
    text-decoration: none;
    font-size: 1.8rem;
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



@media (max-width: 900px) {

  body {
    overflow-y: visible;
  }


  #app {
  display: flex;
  flex-direction: column;
}
  #nav {
    padding: 1rem;
    height: 10rem;
    width: 100vw;
    max-width: 100%;

  a {
    font-size: 2rem;
  }

    .menu {
      flex-direction: row;
    padding: 1rem;
    gap: 5rem;
  }
  }

  
}
</style>
