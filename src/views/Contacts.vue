<template>
  <section id="contacts">
      <div class="contacts-container">
        <div>
          <img src="../.././public/img/bg-contact.svg" alt="imagem de email de contato">
        </div>

        <h1>Fale Comigo!</h1>
        
        <ul>
          <li>
              <a href="https://www.linkedin.com/in/marcos-cantarutti/" target="_blank">
                <i class="fab fa-linkedin"></i>
              </a>
            </li>
          <li>
            <a href="https://github.com/MarcosCantarutti" target="_blank">
              <i class="fab fa-github-square"></i>
            </a>
            </li>
          <li>
            <a href="mailto:marcossandim21@gmail.com">
                <i class="fas fa-envelope-square"></i>
            </a>
          </li>
        </ul>
        <button type="submit">
          <a href="./src./assets/MarcosCantarutti.pdf" download>Download CV</a>
        </button>
        
        
      </div>
  </section>
</template>

<script>


export default {
  name: 'Contacts',
  components: {
  
  }
}
</script>


<style lang="scss" scoped>

  #contacts{
    width: 100%;
    margin: auto 0;
    text-align: center;
    display: flex;
    align-items: center;
    justify-content: center;
    
    

    .contacts-container{
      background-color: #212121;
      padding: 5rem;
      width: 40rem;
      height: 60rem;
      border-radius: 1rem;
      margin: 0 auto;
      -webkit-box-shadow: inset -1px 3px 8px 5px #554BFF, 2px 5px 16px 0px #554BFF, 1px 1px 1px 1px #554BFF; 
      box-shadow: inset -1px 3px 8px 5px #554BFF, 2px 5px 16px 0px #554BFF, 1px 1px 1px 1px #554BFF;
      ul,li {
        list-style: none;

      }
      a{
        text-decoration: none;
        color: #fff;
        font-size: 2rem;
        cursor: pointer;
      }

      i{
        color: #fff;
        font-size: 4rem;
        margin-right: 1rem;
        transition: .3s ease-out;
        &:hover{
          color: #554BFF;
          transform: translate(0, -5px);

        }
      }
      h1 {
        font-size: 3rem;
        color: #fff;
      }

      ul {
        display: flex;
        margin: 5rem auto 0;
        align-items: center;
        justify-content: center;
        gap: 3rem;
      }

      button {
        display: block;
        text-align: left;
        background-color: #554BFF;
        margin: 5rem auto;
        padding: 2rem;
        font-size: 2rem;
        border: none;
        border-radius: 1rem;
        transition: .3s ease-out;
        font-weight: bold;
        &:hover{
          background-color: #fff;
          a{
          color: #212121;
          }
          transform: scale(1.1)
        }
        
      
      }
      img {
        width: 80%;
        margin-bottom: 2rem;
      }
    }

     @media (max-width: 880px) {
       .contacts-container {
        margin: 10rem auto;
       }
     }

    @media (max-width: 690px) {
      #contacts{
      width: 100%;
      height: auto;
      margin: 0 auto;
    }
      .contacts-container {
        margin: 10rem auto;
        padding: 5rem;
        width: 30rem;
        height: 50rem;

         i, h1{
        font-size: 2.5rem;
      }
        button {
          padding: 1.5rem;
          font-size: 1.5rem;
        }
        button a{
          font-size: 1.5rem;
          
        }
      }
     
    }

  }
</style>