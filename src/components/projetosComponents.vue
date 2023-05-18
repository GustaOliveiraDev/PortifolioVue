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
                <div class=" text-normal-projetos">
                    <q-btn flat round dense icon="fa-brands fa-square-github" />
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
                <div class=" text-normal-projetos">
                    <q-btn flat round dense icon="fa-brands fa-square-github" />
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
    margin-left: 10em;
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
    background-image: url('../../public/imgs/projetos/calculadoraOPACA.png');
    background-position: center;
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


@media (max-width: 900px) {

    .conteinerProjetos {

        flex-direction: column;
    }

    .cardProjetosCalculadora {
       
        margin-bottom: 1em;
        margin-left: 0;
    }

    .cardProjetosRelogio {
       
        margin: 0;
    }







}
</style>
  