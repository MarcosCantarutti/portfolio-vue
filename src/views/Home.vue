<template>
  <section class="about">
    <div class="container-about">
         <TypeEffect/>
         
         <div class="container-text">
           <h2>Sobre mim</h2>
           <p>Olá! meu nome é Marcos, trabalho na área da informática desde 2014 em manutenções e atendimento ao cliente, desde o inicio de 2021 iniciei o aprofundamento nos meus estudos com foco no desenvolvimento de aplicações web/landing pages.</p>

          <p>Atualmente sou estudante de Análise e Desenvolvimento de Sistemas na Uninter, também tenho estudado através de cursos com foco na minha especialização.</p> 
          <p>
            Tenho interesse hoje em desenvolvimento web e estou explorando no momento o JavaScript voltado para o Front End, estudo nas plataformas dos cursos da Rocketseat, Origamid, Udemy e CJRM 
          </p>
          <p>
            Recentemente iniciei os estudos com Vue JS e SASS, onde apliquei na construção dessa página =D.
            Porém sempre aberto para aprender novas tecnologias/ferramentas em busca de novas oportunidades.
          </p>


         </div>
    </div>
  </section>
</template>


<script>
import TypeEffect from '../components/TypeEffect.vue'
export default {
  name: 'Home',

  components: {
    TypeEffect,

  }
}
</script>

<style lang="scss" scoped>

  $background: #212121;
 
  .about {
   color: #fff;
    width: 100%;
   display: flex;
   align-items: center;
   justify-content: center;
  }

  .container-about {
    width: 80%;
    height: 80rem;
    
    h1{
      font-size: 4rem;
      text-align: left;
      padding: 5rem;
    }

  
}

.container-text {
    display: flex;
    width: 70%;
    height: auto;
    justify-content: left;
    align-items: flex-start;
    flex-direction: column;
    gap: 2rem;
    
    margin: 15rem 5rem;
    h2 {
      font-size: 3.5rem;
      color: #554BFF;
      font-weight: normal;
    }

    p {
      font-size: 2rem;
      text-align: left;
      letter-spacing: 0.1rem;
    }
  }
</style>