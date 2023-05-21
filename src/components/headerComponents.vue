<template>
  <div class="headerContainer">

    <img class="imgHarder" src="../../public/imgs/LOGOG.png" alt="logo">

    <div class="menuWeb">
      <div class="rotasWeb">Home</div>
      <div class="rotasWeb">Atuação</div>
      <div class="rotasWeb">Contato</div>
      <div class="rotasWeb">Sobre nós</div>


    </div>

    <div class="menuMobile">
      <toogleMenu />
    </div>

  </div>
</template>

<script>
import { ref } from 'vue';
import toogleMenu from 'src/components/toogleMenu.vue'
export default {

  components: {
    toogleMenu,
  }


}
</script>

<style>
.headerContainer {
  width: 100%;
  height: 100px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #0a192f;
}


.imgHarder {
  height: 50px;
  width: 50px;
}

.menuWeb {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.rotasWeb {
  color: white;
  margin-left: 1em;
  font-size: 20px;
}

.rotasWeb:hover {
  transition: 0.3s;
  color: #00b4ff;

}


.menuMobile {
  display: none;
}


.change-bg {
  width: 520px;
  height: 460px;
  overflow: hidden;
  background-color: red;
  transform: translate(-60%, -30%);
}




@media (max-width: 900px) {
  .rotasWeb {
    display: none;
  }

  .imgHarder {
    position: absolute;
    left: 20px;
    height: 50px;
    width: 50px;
  }

  .menuMobile {
    display: flex;
    cursor: pointer;
    color: #00b4ff;
    margin-left: 1em;
    margin-right: 1em;
    display: block;
    transform: rotate(180deg);
  }

}
</style>
