<template>
  <div id="container-about">
    <div class="conteudoAbout-text">

      <div class="text-titulo-about">
        Sobre min
      </div>

      <div class=" text-normal-about">
        Olá! Meu nome é Brittany e gosto de criar coisas que vivem na internet.
        Meu interesse em desenvolvimento web começou em 2012,

      </div>

      <div class=" text-normal-about">
        Avançando para hoje, tive o privilégio de trabalhar na uma agência de publicidade,]

      </div>

      <div class=" text-normal-about">
        eu também recentemente lançou um curso que abrange tudo o
        que você precisa para criar um aplicativo da web com

      </div>

      <div class="tecnologias-about">

        <div class="tec-container">
          <div class="tec">
            <q-icon class="tec-icon" name="fa-solid fa-circle-right" />
            JavaScript
          </div>

          <div class="tec">
            <q-icon class="tec-icon" name="fa-solid fa-circle-right" />
            Reagir
          </div>

          <div class="tec">
            <q-icon class="tec-icon" name="fa-solid fa-circle-right" />
            TypeScript
          </div>

        </div>


        <div class="tec-container">
          <div class="tec">
            <q-icon class="tec-icon" name="fa-solid fa-circle-right" />
            WordPress
          </div>
          <div class="tec">
            <q-icon class="tec-icon" name="fa-solid fa-circle-right" />
            Node.js
          </div>
          <div class="tec">
            <q-icon class="tec-icon" name="fa-solid fa-circle-right" />
            Eleventy
          </div>
        </div>
      </div>

    </div>

    <div class="about-container">
      <img class="about-img" src="../../public/imgs/AdobeStock_550513538_Preview.png">
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
  height: 80vh;
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
  margin-right: 0.5rem;
  margin-bottom: 1rem;
}

.tec-icon {
  margin-right: 0.5rem;
}

.tec:hover {
  transition: 0.3s;
  color: white;
}

@media (max-width: 900px) {
  .container-about {
    flex-direction: column;
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

  }


}
</style>
