<template>
  <div id="containerContato">


    <div class="text-titulo-contato">
      Contato
    </div>

    <div class="text-normal-contato">
      Entre em contato para discutir suas necessidades e trabalharmos juntos em uma solução personalizada.
      Estou animado para colaborar e transformar suas ideias em realidade!
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
#containerContato {
  height: 100vh;
  width: 85vw;
  display: flex;
  justify-content: center;
  transition: 0.3s ease;
  align-items: center;
  text-align: center;
  flex-direction: column;
}


.text-titulo-contato {
  font-size: clamp(50px, 50px + 50px, 20px);
  color: white;
}

.text-normal-contato {
  font-size: clamp(16px, 16px + 16px, 16px);
  color: #00b4ff;
}

@media (max-width: 700px) {

  #containerContato {
    flex-direction: column;
    align-items: center;

    height: 400px;
    width: 85vw;
  }


}
</style>
