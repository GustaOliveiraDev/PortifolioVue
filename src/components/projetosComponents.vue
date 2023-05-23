<template>
  <div id="conteinerProjetos">
    <div class="lineProjetos">

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
            Relógio

          </div>
          <div class="projetosIcon"><a href="https://github.com/GustaOliveiraDev/Relogio-Analogico-Vuejs" target="_blank">
              <q-icon size="xl" name="fa-brands fa-square-github" />
            </a>
          </div>
        </div>

      </div>
    </div>

    <div class="lineProjetos">

      <div class="cardProjetosCep">

        <div class="carLeftCep">
          <div class=" text-normal-projetos">
            HTML CSS JS REACT
          </div>
          <div class="text-titulo-projetos">
            Buscar cep

          </div>
          <div class="projetosIcon"><a href="https://github.com/GustaOliveiraDev/BuscadorCep" target="_blank">
              <q-icon size="xl" name="fa-brands fa-square-github" />
            </a>
          </div>
        </div>

      </div>

      <div class="cardProjetosPortir">

        <div class="cardRightPortir">
          <div class=" text-normal-projetos">
            HTML CSS JS VUEJS QUASAR
          </div>
          <div class="text-titulo-projetos">
            Portifolio

          </div>
          <div class="projetosIcon"><a href="https://github.com/GustaOliveiraDev/PortifolioVue" target="_blank">
              <q-icon size="xl" name="fa-brands fa-square-github" />
            </a>
          </div>
        </div>

      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: [
    'tec',
    'titulo',
    'img',
    'git',

  ]
}
</script>

<style>
#conteinerProjetos {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  transition: 0.3s ease;
  height: 1000px;
  width: 85vw;
}

.lineProjetos {
  display: flex;
  margin-bottom: 3em;
  justify-content: center;
  align-items: center;
  transition: 0.3s ease;
}




.cardProjetosCalculadora {
  width: 360px;
  height: 360px;
  display: flex;
  background-color: #0a192f;
}

.cardProjetosRelogio {
  margin-left: 3em;
  width: 360px;
  height: 360px;
  display: flex;
  background-color: #0a192f;
}

.cardProjetosCep {
  width: 360px;
  height: 360px;
  display: flex;
  background-color: #0a192f;
}

.cardProjetosPortir {
  margin-left: 3em;
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

.carLeftCep {
  margin-bottom: 2em;
  border-right: 2px solid #00b4ff;
  background-image: url('../../public/imgs/projetos/busacadorCep.png');
  background-position: center;
}

.cardRightPortir {
  margin-bottom: 2em;
  border-right: 2px solid #00b4ff;
  background-image: url('../../public/imgs/projetos/PotifolioVue.png');
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

.carLeftCep {
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

.cardRightPortir {
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
    height: 1200px;
    width: 85vw;

  }


  .lineProjetos {
    flex-direction: column;
  }

  .cardProjetosCalculadora {
    width: 250px;
    height: 250px;
    margin-bottom: 1em;
    margin-left: 0;
  }


  .carLeftCalculadora {

    width: 250px;
    height: 250px;

  }

  .cardProjetosRelogio {
    width: 250px;
    height: 250px;
    margin: 0;
  }


  .cardRightRelogio {

    width: 250px;
    height: 250px;

  }


  .cardProjetosCep {
    width: 250px;
    height: 250px;
    margin-bottom: 1em;
    margin-left: 0;
  }


  .carLeftCep {

    width: 250px;
    height: 250px;

  }

  .cardProjetosPortir {
    width: 250px;
    height: 250px;
    margin-bottom: 0;
    margin: 0;
  }


  .cardRightPortir {

    width: 250px;
    height: 250px;

  }







}
</style>
