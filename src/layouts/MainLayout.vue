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

            <q-icon size="sm" name="fa-solid fa-bars-staggered" />



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

          <q-item clickable>
            <q-item-section class="rotasDrawer">
              <div> <a href="#containerApresentacao">
                <q-icon size="sm" name="fa-brands fa-square-github" />
                Olá
              </a></div>
            </q-item-section>
          </q-item>

          <q-item clickable >
            <q-item-section>
              <div class="rotasDrawer"><a href="#container-about">
                <q-icon size="sm" name="fa-solid fa-address-card" />
                Sobre
              </a></div>
            </q-item-section>
          </q-item>

          <q-item clickable>
            <q-item-section>
              <div class="rotasDrawer"><a href="#container-trabalho">
                <q-icon size="sm" name="fa-solid fa-mountain" />
                Experiencias
              </a></div>
            </q-item-section>
          </q-item>

          <q-item clickable>
            <q-item-section>
              <div class="rotasDrawer"><a href="#conteinerProjetos">
                <q-icon size="sm" name="fa-solid fa-diagram-project" />
                Projetos
              </a></div>
            </q-item-section>
          </q-item>

          <q-item clickable>
            <q-item-section>
              <div class="rotasDrawer"><a href="#containerContato">
                <q-icon size="sm" name="fa-solid fa-address-book" />
                Contato
              </a></div>
            </q-item-section>
          </q-item>


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


export default {

  setup() {
    let drawer = ref(false)

    return {
      drawer,
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
  transition: 0.5s;
  cursor: pointer;
  color: #00b4ff;
}

.rotasDrawer{
  color: white;
  transition: 0.5;
  text-decoration: none;
}

.rotasDrawer a{
  color: white;
  transition: 0.5;
  text-decoration: none;
}

.rotasDrawer a:hover {
  transition: 0.3s;
  cursor: pointer;
  color: #00b4ff;
}

.logo {
  height: 50px;
  width: 50px;
  background: #0a192f;
  -webkit-filter: drop-shadow(15px 10px 5px rgba(0, 0, 0, .5));
    filter: drop-shadow(15px 10px 5px rgba(0, 0, 0, .5));
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




}
</style>
