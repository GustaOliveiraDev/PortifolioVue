<template>
  <div id="conteinerProjetos">
    <div class="cardProjetosCalculadora">

      <div class="carLeftCalculadora">
        <div class=" text-normal-projetos">
          HTML CSS JS VUEJS
        </div>
        <div class="text-titulo-projetos">
          Calculadora

        </div>
        <div class="projetosIcon"><a href="https://github.com/GustaOliveiraDev/Calculadora-Vuejs" target="_blank">
            <q-icon size="xl" name="fa-brands fa-square-github" />
          </a>
        </div>
      </div>

    </div>

    <div class="cardProjetosRelogio">

      <div class="cardRightRelogio">
        <div class=" text-normal-projetos">
          HTML CSS JS VUEJS
        </div>
        <div class="text-titulo-projetos">
          Relogio

        </div>
        <div class="projetosIcon"><a href="https://github.com/GustaOliveiraDev/Relogio-Analogico-Vuejs" target="_blank">
            <q-icon size="xl" name="fa-brands fa-square-github" />
          </a>
        </div>
      </div>

    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
#conteinerProjetos {
  display: flex;
  justify-content: center;
  align-items: center;
  transition: 0.3s ease;
  height: 100vh;
  width: 85vw;
}

.cardProjetosCalculadora {
  width: 360px;
  height: 360px;
  display: flex;
  background-color: #0a192f;
}

.cardProjetosRelogio {
  margin-left: 5em;
  width: 360px;
  height: 360px;
  display: flex;
  background-color: #0a192f;
}

.carLeftCalculadora {
  margin-bottom: 2em;
  border-right: 2px solid #00b4ff;
  background-image: url('../../public/imgs/projetos/calculadoraOPACA.png');
  background-position: center;
}

.cardRightRelogio {
  margin-bottom: 2em;
  border-right: 2px solid #00b4ff;
  background-image: url('../../public/imgs/projetos/relogiOpaco1.png');
  background-position: center;
}

.projetosIcon a {
  color: white;
}


.projetosIcon a:hover {
  transition: 0.3s;
  color: #00b4ff;

}

.text-titulo-projetos {
  font-size: clamp(30px, 36px + 36px, 36px);
  color: white;
}

.text-normal-projetos {
  font-size: clamp(16px, 16px + 16px, 16px);
  text-align: start;
  color: #00b4ff;
}

.carLeftCalculadora {
  margin-left: 0em;
  width: 360px;
  height: 360px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  text-align: start;
  border-radius: 25px;
  border-left: 2px solid #00b4ff;
}

.cardRightRelogio {
  margin-left: 0em;
  width: 360px;
  height: 360px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  text-align: start;
  border-radius: 25px;
  border-left: 2px solid #00b4ff;
}

/* mix-blend-mode: multiply; */


@media (max-width: 700px) {

  #conteinerProjetos {
    flex-direction: column;
    align-items: center;
    height: 600px;
    width: 85vw;

  }

  .cardProjetosCalculadora {
    width: 250px;
    height: 250px;
    margin-bottom: 1em;
    margin-left: 0;
  }
  .cardRightRelogio {

  width: 250px;
  height: 250px;

}

  .cardProjetosRelogio {
    width: 250px;
    height: 250px;
    margin: 0;
  }

  .carLeftCalculadora {

  width: 250px;
  height: 250px;

}






}
</style>
