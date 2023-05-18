<template>
  <q-page class="flex flex-center primario ">
    <div class="container">

      <sociaisIcon />

      <apresentacaoComponent />
      <sobreComponent />
      <empregosComponents />
      <projetosComponents />
      <contatoComponent />
 
      <sociaisEmail />

   

    </div>
  </q-page>
</template>

<script>

import sociaisIcon from 'src/components/sociaisIcon.vue';
import sociaisEmail from '../components/sociaisEmail.vue';


import apresentacaoComponent from 'src/components/apresentacaoComponent.vue';
import sobreComponent from 'src/components/sobreComponent.vue';
import empregosComponents from 'src/components/empregosComponents.vue';
import projetosComponents from '../components/projetosComponents.vue';
import contatoComponent from '../components/contatoComponent.vue';
import sociaisHorizontalComponents from 'src/components/sociaisHorizontalComponents.vue';

export default {
  name: 'IndexPage',
  components: {
    sociaisIcon,

    apresentacaoComponent,
    sobreComponent,
    empregosComponents,
    projetosComponents,
    contatoComponent,
    
    sociaisEmail,
  }
}
</script>
<style>

.container{
  display: flex;
  justify-content: center;
  flex-direction: column;
}

</style>
