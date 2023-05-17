<template>
  <q-page class="flex flex-center primario ">
    <div class="container">

      <!-- <animacaoLoad /> -->

      <sobreComponent />
      <sobreComponent />
      <sobreComponent />
      <sobreComponent />

      <sociaisIcon />
      <sociaisEmail />

    </div>
  </q-page>
</template>

<script>

import sociaisIcon from 'src/components/sociaisIcon.vue';
import sociaisEmail from '../components/sociaisEmail.vue';
import sobreComponent from 'src/components/sobreComponent.vue';
import animacaoLoad from '../../public/animacao/animacaoLoad.vue';

export default {
  name: 'IndexPage',
  components: {
    sociaisIcon,
    sociaisEmail,
    sobreComponent,
    // animacaoLoad,
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
