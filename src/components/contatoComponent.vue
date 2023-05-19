<template>
  <div id="containerContato">


      <div class="text-titulo-contato">
        Contato
      </div>

      <div class="text-normal-contato">
        Um desenvolverdor de software<br>
        especializado em construsir e projeta<br> experiencias excepcionais!
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

@media (max-width: 600px) {
  .conteudoSobre {
    flex-direction: column;
    width: 80vw;
  }

}
</style>
