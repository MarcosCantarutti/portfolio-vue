<template>
  <section id="projects">
      <h1>Meus projetos</h1>
    <Project />
    
    
  </section>
</template>

<script>

import Project from '../components/Project.vue'
export default {
  name: 'Projects',
  components: { 
    Project 
  },

  methods:{

  }
}
</script>


<style lang="scss" scoped>

  h1 {
    font-size: 3rem;
    background: -webkit-linear-gradient(#2E34EA, #554BFF);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin: 1rem auto 0;
    text-align: center;
  }
 
  #projects {
    width: 100%;
    background-color: #181818;
   
  }

   @media (max-width: 800px) {
     h1 {
       margin: 0.5 auto 0;
     }
    #projects {
      height: 100%;
    margin: 0 auto;
     display: flex;
     flex-direction: column;
     align-items: center;
     justify-content: center;
     gap: 1.5rem;
  }

     h1 {
    font-size: 2.5rem;
    }
    
  }

</style>