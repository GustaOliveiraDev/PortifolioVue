<template>

  <div id="container-about">


      <div class="conteudoAbout-text">

        <div class="text-titulo-about">
          Sobre min
        </div>

        <div class=" text-normal-about">
          Olá, sou Gustavo, um programador com experiência em front-end,
           oferecendo serviços de freelancer para projetos web e mobile.

        </div>

        <div class=" text-normal-about">
          Tenho conhecimentos em JavaScript, Vue.js e React,
           e experiência em integração de APIs e
          criação de interfaces de usuário interativas e responsivas.

        </div>

        <div class=" text-normal-about">
          Com um portfólio online destacando minhas habilidades,
         sou comprometido em entregar resultados de alta qualidade e cumprir prazos.
        </div>

        <div class="tecnologias-about">

          <div class="tec-container">
            <div class="tec">
              <q-icon class="tec-icon" name="fa-solid fa-circle-right" />
              JavaScript
            </div>

            <div class="tec">
              <q-icon class="tec-icon" name="fa-solid fa-circle-right" />
              React
            </div>

            <div class="tec">
              <q-icon class="tec-icon" name="fa-solid fa-circle-right" />
              APIs
            </div>

          </div>


          <div class="tec-container">
            <div class="tec">
              <q-icon class="tec-icon" name="fa-solid fa-circle-right" />
              TypeScript
            </div>
            <div class="tec">
              <q-icon class="tec-icon" name="fa-solid fa-circle-right" />
              Vue
            </div>
            <div class="tec">
              <q-icon class="tec-icon" name="fa-solid fa-circle-right" />
              Quasar
            </div>
          </div>
        </div>

      </div>
      <div class="about-container">
        <img class="about-img" src="../../public/imgs/FOTOF.png">
      </div>



    </div>

</template>

<script>
export default {

}
</script>

<style>
#container-about {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  width: 85vw;
}

.about-container {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-left: 1rem;
  background-color: #0a192f;
}

.about-img {
  width: 310px;
  height: 310px;
  background-color: #00b4ff;
  transition: 0.3s;
  box-shadow: 10px 10px 0px #00b4ff;
}

.about-img:hover {
  transition: 0.3s;
  margin-bottom: 20px;
  margin-right: 20px;
  box-shadow: 30px 30px 0px #00b4ff;
}

.conteudoAbout-text {
  align-items: start;
  width: 50vw;
}

.text-titulo-about {
  font-size: clamp(40px, 40px + 40px, 40px);
  color: #00b4ff;
}

.text-normal-about {
  font-size: clamp(16px, 16px + 16px, 16px);
  margin-bottom: 1rem;
  color: white;
}

.tecnologias-about {
  display: flex;
  justify-content: center;
  align-items: center;
  color: #00b4ff;
  margin-bottom: 1rem;
}

.tec-container {
  display: flex;
  margin-right: 5rem;
  justify-content: center;
  flex-direction: column;
}

.tec {
  display: flex;
  align-items: center;
  /* margin-right: 0.5rem; */
  margin-bottom: 1rem;
}

.tec-icon {
  margin-right: 0.5rem;
}

.tec:hover {
  transition: 0.3s;
  color: white;
}

@media (max-width: 700px) {

  #container-about {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    transition: 0.3s ease;
  }

  #container-about {
  height: 1000px;
  width: 85vw;

}

  .tec-container {
    display: flex;
    margin-right: 0.5em;

  }

  .conteudoAbout-text {
    width: 85vw;

  }

  .text-normal-about {
    text-align: center;
  }

  .text-titulo-about {
    text-align: center;
  }

  .conteudoAbout-img {
    width: 150px;
    height: 150px;
  }

  .about-img {
    width: 200px;
    height: 200px;
    margin: 0;
    background-color: #00b4ff;
    box-shadow: 10px 10px 0px #00b4ff;
  }

  .about-container {
    margin-left: 0;
    margin-right: 1em;

  }


}
</style>
