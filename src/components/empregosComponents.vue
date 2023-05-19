<template>
    <div id="container-trabalho">
        <div class="conteudoTrabalho">

            <div class="titulo-trabalho">
                Trabalhos
            </div>


                <div class="trabalhos">

                    <div class="text-titulo-trabalho">
                        <q-icon class="trabalho-icon" name="fa-solid fa-circle-right" />
                        Freelacers
                    </div>
                    <div class="text-normal">
                        2021-2023<br>
                    </div>

                </div>
                <div class="lineHorizontal">

                </div>
                <div class="trabalhos">

                    <div class="text-titulo-trabalho">
                        <q-icon class="trabalho-icon" name="fa-solid fa-circle-right" />
                        Estagio
                    </div>
                    <div class="text-normal">
                        2021-2023<br>

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
#container-trabalho {
    height: 80vh;
    width: 85vw;
    display: flex;
    justify-content: center;
    transition: 0.3s ease;
    align-items: center;
}

.titulo-trabalho {
    font-size: clamp(40px, 40px + 40px, 40px);
    color: #00b4ff;
    margin-bottom: 1em;
    text-align: center;
}

.conteudoTrabalho {
    flex-direction: column;
    display: flex;
    justify-content: center;
    align-items: center;
}

.lineHorizontal {
    height: 200px;
    width: 1px;
    border-left: 1px solid #00b4ff;
}

.trabalho-icon {
    color: #00b4ff;
}

.text-titulo-trabalho {
    font-size: clamp(26px, 26px + 26px, 26px);
    text-align: center;
    color: white;
}


.text-normal {
    font-size: clamp(16px, 16px + 16px, 16px);
    text-align: center;
    color: #00b4ff;
}

@media (max-width: 900px) {

    .conteudoSobre {
        width: 80vw;
    }

    .titulo-trabalho {
        width: 250px;

    }

    .line-trabalho {
        border: none;
}

.text-titulo-trabalho {
   text-align: center;
}

.text-normal {
    text-align: center;
}


}
</style>
