<template> 
  <div>

    <div class="card">    
        
      <p>Projeto: <a :href="urlLink" target="_blank"> {{title}}</a></p>
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
 $colorsText: #ffffff;
  .card{
        color: rgb(184, 184, 184);
        font-size: 1.5rem;
        padding: 1.5rem;
        width: 40rem;
        height: 18rem;
        border-radius: 1rem;
        background-color: #010101;
        transition: .3s ease-out;
        a {
          text-decoration: none;
          color: $colorsText;
        }

        &:hover{
          -webkit-box-shadow: 0px 10px 13px -7px #000000, 5px 5px 15px 5px rgba(0,0,0,0.5); 
          box-shadow: 0px 10px 13px -7px #000000, 5px 5px 15px 5px rgba(0,0,0,0.5);
        }
    }

    @media (max-width: 1220px) {
      .card{
        font-size: 1.2rem;
        padding: 1.2rem;
        width: 30rem;
        height: 18rem;
      }
    }
    

    @media (max-width: 830px) {
      .card{
        font-size: 1.2rem;
        padding: 1.2rem;
        width: 20rem;
        height: 18rem;
      }
    }

  
</style>
