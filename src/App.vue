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

$background: #F1F1E7;
$background-routers: #F1F1E7;
$colorsText: #686565;

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
  
  
}

h1, h2, h3 {
  font-weight: 700;
}

#app {
  display: flex;
  min-height: 100vh;
}


#nav {
  
  max-width: 30rem;
  height: auto;
  background: $background-routers;
  display: flex;
  padding: 5rem;
  
  border-right: 3px solid #010101;
 
  a {
    text-decoration: none;
    font-size: 1.8rem;
    font-weight: bold;
    color: $colorsText;

    &.router-link-exact-active {
      color: #010101;
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
  #app {
  display: flex;
  flex-direction: column;
  
}
  #nav {
    padding: 1rem;
    
    width: 100vw;
    max-width: 100%;
    height: auto;
    border-right: 0;
    border-bottom: 3px solid #010101;
    display: flex;
    align-items: center;
    
  a {
    font-size: 1.6rem;
  }

    .menu {
    margin: 0 auto;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    padding: 1rem;
    gap: 2rem;
  }
  }

  
}
</style>
