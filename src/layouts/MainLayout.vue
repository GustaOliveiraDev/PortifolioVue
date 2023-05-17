<template>
  <q-layout>

    <!-- <animacaoLoad /> -->

    <q-header ref="headerL" elevated class="row col-12 col-md-12 headerr ">
      <q-toolbar class="flex primarioText justify-between">

        <q-avatar class="logo">
          <img src="../../public/imgs/AdobeStock_550513538_Preview.png">

        </q-avatar>

        <nav class="menu">
          <div class="links">
            <div class="rotas">Sobre</div>
            <div class="rotas">Expêriencia</div>
            <div class="rotas">Trabalhos</div>
            <div class="rotas">Contato</div>
            <div class="middle">
              <a class="btn btn4">Currículo</a>
            </div>
          </div>

          <div class="toogueMenu">
            <q-btn @click="drawer = !drawer" round icon="menu" />
          </div>
        </nav>

      </q-toolbar>
    </q-header>

    <q-drawer class="drawer" v-model="drawer" :width="200" side="right">

      <q-scroll-area class="fit">
        <q-list >

          <div class="middle">
            <a class="btn btn4">Currículo</a>
          </div>
          <template v-for="(menuItem, index) in menuList" :key="index">
            <q-item class="flex intems-center itemDrawer " v-ripple>

              <q-item-section avatar>
                <q-icon :name="menuItem.icon" />
              </q-item-section>

              <q-item-section>
                {{ menuItem.label }}
              </q-item-section>

            </q-item>
          </template>

        </q-list>
      </q-scroll-area>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>

  </q-layout>
</template>

<script>

import { ref, } from 'vue'
import animacaoLoad from '../../public/animacao/animacaoLoad.vue';

const menuList = [
  {
    icon: 'fa-solid fa-address-card',
    label: 'Sobre',
    separator: false
  },
  {
    icon: 'fa-solid fa-mountain',
    label: 'Expêriencia',
    separator: false
  },
  {
    icon: 'fa-solid fa-diagram-project',
    label: 'Trabalhos',
    separator: false
  },
  {
    icon: 'fa-solid fa-address-book',
    label: 'Contatos',
    separator: true
  },


]

export default {
  setup() {
    let drawer = ref(false)

    return {
      drawer,
      menuList
    }
  },

  components: {
    // animacaoLoad,
  }

}

</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Courier+Prime&display=swap');

* {
  font-family: 'Courier Prime', monospace;
  font-size: 16px;
}

.headerr {
  height: 100px;
  position: fixed;

  background-color: #0a192f;
}

.toogueMenu {
  display: none;
}

.drawer {
  color: #00b4ff;
  background-color: #0a192f;
}

.separador {

  background-color: #00b4ff;
}

.headerRelative {
  background-color: red;
}

.logo {
  height: 50px;
  width: 50px;
  background: #00b4ff;
}

.primario {
  background: #0a192f;
}

.primarioText {
  color: #00b4ff;
}

.header {
  height: 100px;
  position: fixed;
  background: #0a192f;
}

.transition {
  opacity: 0;
  background: #00b4ff;
}

.menu {
  display: flex;
  justify-content: center;
  align-items: center;

}

.links {
  display: flex;
  justify-content: center;
  align-items: center;
}

.rotas {
  padding-right: 25px;
  color: white;
}

.rotas:hover {
  transition: 0.3s;
  cursor: pointer;
  color: #00b4ff;
}

.logo {
  height: 50px;
  width: 50px;
  background: #00b4ff;
}

.logo:hover {
  -webkit-filter: drop-shadow(15px 10px 5px rgba(0, 0, 0, .5));
  filter: drop-shadow(15px 10px 5px rgba(0, 0, 0, .5));
}


.btn {
  position: relative;
  display: flex;
  color: white;
  font-size: 14px;
  text-decoration: none;
  border: 1px solid #00b4ff;
  padding: 10px;
  overflow: hidden;
  border-radius: 10px;
  transition: 1s all ease;
}

.btn::before {
  background: #00b4ff;
  content: "";
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  z-index: -1;
  transition: all 0.6s ease;
}

.btn4::before {
  width: 100%;
  height: 0%;
  transform: translate(-50%, -50%) rotate(-45deg);
}

.btn4:hover::before {
  height: 380%;
}

@media (max-width: 600px) {
  .toogueMenu {
    display: block;
  }

  .links {
    display: none;
  }

  .itemDrawer {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-bottom: 30px;


  }


  .middle {
    display: flex;
    justify-content: center;
  }

  .btn {
    width: 150px;
    margin: 25px;
    /* margin-top: 30px;
    margin-bottom: 150px; */
  }



}
</style>
