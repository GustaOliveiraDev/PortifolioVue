<template>
    <div class="containerSocialEmail">

        <div class="socialEmail">

            <div round class="socialTexEmail" @click="enviarEmail">
                GustaOliveiraDev@gmail.com
            </div>

        </div>

        <div class="socialLineEmail">
            <div>
            </div>
        </div>

    </div>
</template>
  
<script>
export default {
    methods: {
        enviarEmail() {
            window.location.href = `mailto:?body=Olá, entrei no endereço  e econtrei a norma
              nº  - MT, gostaria de compartilha-la com você, para acessá-lá clique no link: `;
        },
    }
}
</script>
  
<style>
.containerSocialEmail {
    position: fixed;
    right: 50px;
    bottom: 0px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}

.socialEmail {
    height: 150px;
    color: white;
}

.socialTexEmail {
    display: flex;
    justify-content: center;
    align-items: center;
    transform: rotate(90deg);
    cursor: pointer;
    width: 30px;
}

.socialTexEmail:hover {
    transition-duration: 0.3s;
    color: #00b4ff;
    padding-right: 10px;
}

.socialLineEmail {
    border-right: 1px solid;
    height: 200px;
    color: white;
}

@media (max-width: 600px) {

    .containerSocialEmail {
        display: none;
    }



}
</style>