<template>
  <div id="containerApresentacao">

    <transition :duration="10000" appear active-class="animated fadeInUp" leave-active-class="animated fadeOutUp">
    <div class="paiApresentacao" data-animation="top">

      <div class="text-normal">
        Olá!
      </div>

      <div class="text-titulo">
        Prazer, sou o Gustavo.
      </div>

      <div class="text-normal">
        Um programador com experiência em desenvolvimento front-end
      </div>

      <sociaisHorizontal />

    </div>
    </transition>

  </div>
</template>

<script>
import sociaisHorizontal from 'src/components/sociaisHorizontalComponents.vue'

export default {
  components: {
    sociaisHorizontal,
  },


}
</script>

<style>
#containerApresentacao {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  height: 600px;
  width: 85vw;
}

.paiApresentacao {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}


.text-titulo {
  font-size: clamp(50px, 50px + 50px, 20px);
  color: white;
  text-align: center;

}

.text-normal {
  font-size: clamp(16px, 16px + 16px, 16px);
  color: #00b4ff;
}

@media (max-width: 350px) {

  #containerApresentacao {
  flex-direction: column;
  align-items: center;
  height: 300px;
  width: 85vw;
}
  .conteudoSobre {
    flex-direction: column;
    text-align: center;

  }

  .text-titulo {
    font-size: clamp(26px, 26px + 26px, 26px);
    color: white;
  }

  .text-normal {
    font-size: clamp(16px, 16px + 16px, 16px);
    text-align: center;
    color: #00b4ff;
  }

}

</style>
