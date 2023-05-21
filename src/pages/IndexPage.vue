<template>
  <q-page class="flex flex-center primario ">
    <div class="container">

      <sociaisIcon />

      <apresentacaoComponent />
      <sobreComponent />
      <experienciaComponents />
      <projetosComponents />
      <contatoComponent />

      </div>

      <sociaisEmail />

  </q-page>
</template>

<script>

import sociaisIcon from 'src/components/sociaisIcon.vue';
import sociaisEmail from '../components/sociaisEmail.vue';
import { ref, computed } from 'vue'

import apresentacaoComponent from 'src/components/apresentacaoComponent.vue';
import sobreComponent from 'src/components/sobreComponent.vue';
import experienciaComponents from 'src/components/experienciaComponents.vue';
import projetosComponents from '../components/projetosComponents.vue';
import contatoComponent from '../components/contatoComponent.vue';


export default {
  name: 'IndexPage',
  components: {
    sociaisIcon,

    apresentacaoComponent,
    sobreComponent,
    experienciaComponents,
    projetosComponents,
    contatoComponent,

    sociaisEmail,
  },


}
</script>
<style >
html {
  scroll-behavior: smooth;
}

.container {
  display: flex;
  justify-content: center;
  flex-direction: column;
}
</style>
