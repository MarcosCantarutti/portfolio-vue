<template> 
  <div>

    <div class="card">    
        
      <p>Projeto: <a :href="urlLink"> {{title}}</a></p>
      <p>Descrição: {{description}}</p>
    </div>

  </div>
</template>

<script>
export default {
  name: 'Card',
  props: {
    title: String,
    description: String,
    urlLink: String,
  }
}
</script>

<style lang="scss" scoped>
  .card{
        color: #fff;
        font-size: 1.5rem;
        padding: 1.5rem;
        width: 40rem;
        height: 18rem;
        border-radius: 1rem;
        background-color: #212121;
        a {
          text-decoration: none;
          color: #554BFF;
        }
    }
    

    @media (max-width: 830px) {
      .card{
        font-size: 1rem;
        padding: 1.2rem;
        width: 15rem;
        height: 18rem;
      }
    }

  
</style>
