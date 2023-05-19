<template>
  <q-layout>


    <q-header class="row col-12 col-md-12 headerr ">
      <q-toolbar class="flex primarioText justify-between">

        <q-avatar class="logo">
          <img src="../../public/imgs/LOGOG.png">

        </q-avatar>

        <nav class="menu">
          <div class="links">

            <transition appear enter-active-class="animated fadeInDown" leave-active-class="animated fadeInDown">
              <div class="rotas"><a href="#containerApresentacao">Olá</a></div>
            </transition>


            <transition appear enter-active-class="animated fadeInDown" leave-active-class="animated fadeInDown">
              <div class="rotas"><a href="#container-about">Sobre</a></div>

            </transition>


            <transition appear enter-active-class="animated fadeInDown" leave-active-class="animated fadeInDown">
              <div class="rotas"><a href="#container-trabalho">Expêriencia</a></div>

            </transition>


            <transition appear enter-active-class="animated fadeInDown" leave-active-class="animated fadeInDown">
              <div class="rotas"><a href="#conteinerProjetos">Trabalho</a></div>

            </transition>


            <transition appear enter-active-class="animated fadeInDown" leave-active-class="animated fadeInDown">
              <div class="rotas"><a href="#containerContato">Contato</a></div>

            </transition>


            <transition appear enter-active-class="animated fadeInDown" leave-active-class="animated fadeInDown">

              <div @click="encaminhePdf()" class="containerBtnCurriculo">
                <a
                  href="https://drive.google.com/file/d/1UhfvvZ381JVe-mXCRIETFyrKmVOiZTJj/view?usp=share_link">Curriculo</a>
              </div>
            </transition>


          </div>

          <div class="toogueMenu" @click="drawer = !drawer">
          
            <q-icon  size="sm" name="fa-solid fa-bars-staggered"/>

         
           
          </div>
        </nav>

      </q-toolbar>
    </q-header>

    <q-drawer class="drawer" v-model="drawer" :width="200" side="right">

      <q-scroll-area class="fit">
        <q-list>

          <div class="containerBtnCurriculo">
            <a class="btnLinkCurriculo">Curriculo</a>
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



}

</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Courier+Prime&display=swap');

* {
  font-family: 'Courier Prime', monospace;
  box-sizing: border-box;
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
  transition: 0.5;
  color: white;
}

.rotas a {
  color: white;
  transition: 0.5;
  text-decoration: none;
}

.rotas a:hover {
  transition: 0.3s;
  cursor: pointer;
  color: #00b4ff;
}

.logo {
  height: 50px;
  width: 50px;
  background: #0a192f;
}

.logo:hover {
  -webkit-filter: drop-shadow(15px 10px 5px rgba(0, 0, 0, .5));
  filter: drop-shadow(15px 10px 5px rgba(0, 0, 0, .5));
}

.containerBtnCurriculo {
  display: flex;
  justify-content: center;
  border: 1px solid #00b4ff;
  padding: 10px;
  border-radius: 25px;
  width: 150px;
  margin: 25px;
  cursor: pointer;
  text-decoration: none;
  color: white;
}

.containerBtnCurriculo a {

  text-decoration: none;
  color: white;
}




@media (max-width: 900px) {
  .toogueMenu {
    display: block;
    transform: rotate(180deg);
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


  .containerBtnCurriculo {
    display: flex;
    justify-content: center;
    border: 1px solid #00b4ff;
    padding: 10px;
    border-radius: 25px;
    width: 150px;
    margin: 25px;
  }

  .btnLinkCurriculo {}



}
</style>
