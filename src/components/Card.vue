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
        height: 20rem;
        border-radius: 1rem;
        background-color: #212121;
        a {
          text-decoration: none;
          color: #554BFF;
        }
    }
    @media (max-width: 1575px) {
      .card{
        font-size: 1.3rem;
        padding: 1.3rem;
        width: 30rem;
        height: 14rem;
      }
    }

    @media (max-width: 1230px) {
      .card{
        font-size: 1.3rem;
        padding: 1.3rem;
        width: 30rem;
        height: 15rem;
      }
    }

    @media (max-width: 1000px) {
      .card{
        font-size: 1.2rem;
        padding: 1.3rem;
        width: 30rem;
        height: 15rem;
      }
    }

    @media (max-width: 830px) {
      .card{
        font-size: 1rem;
        padding: 1.2rem;
        width: 20rem;
        height: 12rem;
      }
    }

    @media (max-width: 655px) {
      .card{
        font-size: 1.2rem;
        padding: 1.2rem;
        width: 20rem;
        height: 15rem;
      }
    }

     @media (max-width: 655px) {
      .card{
        font-size: 1.1rem;
        padding: 1.2rem;
        width: 15rem;
        height: 20rem;
      }
    }

    @media (max-width: 555px) {

      .card{
        font-size: 0.9rem;
        padding: 1.2rem;
        width: 15rem;
        height: 15rem;
      }
    }

    @media (max-width: 520px) {

      .card{
        font-size: 0.9rem;
        padding: 1.2rem;
        width: 14rem;
        height: 16rem;
      }
    }
</style>
