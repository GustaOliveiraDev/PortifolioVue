<template>
  <div id="containerApresentacao">

    <div class="text-normal">
      Meu nome é
    </div>
    <div class="text-titulo">
      Gustavo Oliveira<br>
     E sou desenvolverdor
    </div>

    <div class="text-normal">
  
      especializado em construsir
      e projeta experiencias excepcionais!
    </div>

    <sociaisHorizontal />

  </div>
</template>

<script>
import sociaisHorizontal from 'src/components/sociaisHorizontalComponents.vue'
export default {
  components: {
  sociaisHorizontal,
}
}
</script>

<style>
#containerApresentacao {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  height: 100vh;
  width: 85vw;
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

@media (max-width: 900px) {
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
