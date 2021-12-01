<template>    
    <div v-if="isLoading === true">
        Carregando...
    </div>
    <div v-if="hasError === true">
        Falha
    </div>
    <div v-else>
    <div class="grid">
      <div class="col" v-for="project in data" v-bind:key="project.id">
          
        <Card 
            :title="project.name" 
            :urlLink="project.html_url" 
            :description="project.description">
        </Card>
      </div>
    </div>  
    </div>
</template>

<script>
import Card from './Card.vue'
import axios from 'axios'
export default {
  name: 'Projects',
  components: {
    Card
  },
  data () 
  {
    return {
      data: null,
      isLoading: true,
      hasError: false
    }
  },
  mounted () {
    axios
      .get('https://api.github.com/users/marcoscantarutti/repos', {
        headers: {
          'Accept': 'application/vnd.github.mercy-preview+json'
        }})
      .then(response => (
        this.data = response.data.filter(project => {
          return (
          project.name === 'animaisFantasticos' || 
          project.name === 'beutysaloon' ||
          project.name === 'NLW-HEAT-ORIGIN' ||
          project.name === 'jogo-da-memoria' ||
          project.name === 'JordanShoes' ||
          project.name === 'RocketQ' ||
          project.name === 'Lista-de-tarefas-com-React'||
          project.name === 'make_your_burguer'||
          project.name === 'Portfolio'
        )})
      ))
      .catch(error => {
        console.log(error)
        this.hasError = true
      })
      .finally(() => this.isLoading = false)
  }
}
</script>

<style lang="scss" scoped>


 
  .grid{
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(40rem, 1fr));
    grid-template-rows: auto;
    grid-gap: 2rem;
    padding: 5rem;
  }

    @media (max-width: 900px) {
    
    .grid{
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: auto;
    grid-gap: 2rem;
    padding: 1rem;
    margin: 0 auto;
    }
    
  }


</style>