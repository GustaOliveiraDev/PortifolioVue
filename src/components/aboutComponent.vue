<template>
  <div class="container-about">
    <div class="conteudoAbout-text">

      <div class="text-titulo-about">
        Sobre min
      </div>

      <div class=" text-normal-about">
        Olá! Meu nome é Brittany e gosto de criar coisas que vivem na internet.
        Meu interesse em desenvolvimento web começou em 2012,
        quando decidi tentar editar temas
        personalizados do Tumblr - descobrir que criar um botão de reblog personalizado
        me ensinou muito sobre HTML e CSS!
      </div>

      <div class=" text-normal-about">
        Avançando para hoje, tive o privilégio de trabalhar na uma agência de publicidade,]
        uma start-up, uma grande corporação, e um estúdio de design liderado por estudantes.
        Atualmente, meu foco principal é criar produtos acessíveis
        e inclusivos e experiências digitais emUpstatementpara uma variedade de clientes.
      </div>

      <div class=" text-normal-about">
        eu também recentemente lançou um curso que abrange tudo o
        que você precisa para criar um aplicativo da web com
        a API do Spotify usando Node & React.

        Aqui estão algumas tecnologias com as quais tenho trabalhado recentemente:
      </div>

      <div class="tecnologias-about">

        <div class="tec-container">
          <div class="tec">
            <q-icon class="tec-icon" name="fa-solid fa-circle-right" />
            JavaScript (ES6+)
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
    <div class="conteudoAbout-img">
      <q-card class="about-container-img">
        <img class="about-img" src="../../public/imgs/AdobeStock_550513538_Preview.png">
      </q-card>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
.container-about {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 10rem;


}

.about-img {
  width: 200px;
  height: 200px;
  background-color: #00b4ff;
}

.conteudoAbout-img {
  display: flex;
  justify-content: center;
  align-items: center;
  border: 1px solid #00b4ff;
  background-color: red;
  width: 300px;
  height: 300px;
}

.conteudoAbout-text {
  align-items: start;
  width: 50vw;

}

.text-titulo-about {
  font-size: clamp(36px, 36px + 36px, 36px);
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
  text-align: start;
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

@media (max-width: 600px) {
  .container-about {
    flex-direction: column;
  }

  .conteudoAbout-text {
    width: 80vw;

  }

  .conteudoAbout-img {
    width: 150px;
    height: 150px;
  }

}
</style>
