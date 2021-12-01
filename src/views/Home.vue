<template>
  <section class="about">
    <div class="container-about">
         <TypeEffect/>
         
       
          <div class="container-text">
           <h2><i class="fas fa-stream"></i> Sobre mim</h2>
           <p>Olá! meu nome é Marcos, trabalho na área da informática desde 2014 em manutenções e atendimento ao cliente, desde o começo de 2021 iniciei o aprofundamento nos meus estudos com foco no desenvolvimento de aplicações web/landing pages.</p>

          <p>Atualmente sou estudante de Análise e Desenvolvimento de Sistemas na Uninter, tenho também  estudado através de cursos com foco na minha especialização.</p> 
          <p>
            Tenho interesse hoje em desenvolvimento web e estou explorando no momento o JavaScript voltado para o Front End, estudo nas plataformas dos cursos da Rocketseat, Origamid, Udemy e CJRM 
          </p>
          <p>
            Recentemente iniciei os estudos com Vue JS e SASS, onde apliquei na construção dessa página =D, 
            porém sempre aberto para aprender novas tecnologias/ferramentas em busca de novas oportunidades.
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

 
  .about {
    color: #fff;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  

  .container-about {
    width: 100vw;
    height: 100vh;
    background: linear-gradient( rgba(0, 0, 0, 0.9), rgba(0, 0, 0, 0.8) ), url(../.././public/img/bg-home.jpg) center;
    background-repeat: no-repeat;
    background-size: cover;
}

.container-text {
    display: flex;
    width: 50%;
    height: 100%;
    justify-content: left;
    align-items: flex-start;
    flex-direction: column;
    gap: 2rem;
    margin: 12rem 5rem;

    h2 {
      font-size: 3rem;
      color: #554BFF;
    }

    p {
      font-size: 2rem;
      text-align: left;
      letter-spacing: 0.1rem;
    }

  }

  @media (max-width: 830px) {
  .about {
    color: #fff;
    width: 100%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  

  .container-about {
    width: 100vw;
    height: 100%; 
}

.container-text {
    display: flex;
    width: 80%;
    height: 80%;
    justify-content: left;
    align-items: flex-start;
    flex-direction: column;
    gap: 2rem;
    margin: 5rem 5rem;

    h2 {
      font-size: 2rem;
      color: #554BFF;
    }

    p {
      font-size: 1.6rem;
      text-align: left;
      letter-spacing: 0.1rem;
    }

  }    


}

  
  
</style>