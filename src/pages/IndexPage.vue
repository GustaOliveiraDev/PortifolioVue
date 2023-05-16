<template>
  <q-page class="flex flex-center primario ">

    <div class="container">


      

      <sobreComponent />
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

export default {
  name: 'IndexPage',
  components: {
    sociaisIcon,
    sociaisEmail,
    sobreComponent,
  }
}
</script>
<style>
.container {

  padding: 300px;
}
</style>
