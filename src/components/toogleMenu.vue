<template>
  <div class="menuMobileContainer" @click="toggleActive()">


    <div id="paiMenu">

      <div class="toogleMenu">
        <q-icon size="sm" name="fa-solid fa-bars-staggered" />
      </div>

      <div class="menuMobile" :class="['menuMobile', { 'change': isActive }]">

        <div class="rotasMobile">Home</div>
        <div class="rotasMobile">Atuação</div>
        <div class="rotasMobile">Contato</div>
        <div class="rotasMobile">Sobre nós</div>

      </div>

    </div>

    <div class="menuBg" :class="['menuBg', { 'change-bg': isActive }]"></div>

  </div>
</template>

<script>
import { ref } from 'vue';
export default {

  setup() {
    return {
      isActive: ref(false)
    }
  },

  methods: {

    toggleActive() {
      this.isActive = !this.isActive;
    },

  }
}
</script>

<style>


#paiMenu {
    z-index: 2;
}


#menuMobile {

    display: none;
}

.menuBg, #paiMenu {
    top: 0;
    left: 0;
    position: absolute;
}

.menuBg {
    z-index: 1;
    width: 0;
    height: 0;
    /* margin: 30px 0 20px 20px; */
    border: 1px solid red;
    background: radial-gradient(circle, #00b4ff, #00b4ff);
    border-radius: 50%;
    transition: 0.3s ease;
}

.rotasMobile {
    margin: 15px;
    text-decoration: none;
    color: white;
    font-size: 18px;
}

.rotasMobile a:hover {
    transition: 0.5s ease;
    color: #dcb675;

}

.change {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;

}

.change-bg {
    width: 520px;
    height: 460px;
    overflow: hidden;
    transform: translate(-60%, -30%);
}




</style>
