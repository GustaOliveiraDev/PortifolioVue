<template>
  <q-layout @scroll="handleScroll()">
    <q-header ref="headerL" elevated class="flex headerr ">
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
          </div>


          <div class="middle">
            <a class="btn btn4">Currículo</a>
          </div>

        </nav>

      </q-toolbar>
    </q-header>
    <q-page-container>
      <router-view />

    </q-page-container>

  </q-layout>
</template>

<script>

export default {

  name: 'MainLayout',


  setup() {

    let vet = []
    return {
      vet
    }
  },
  methods: {

    handleScroll() {

      this.vet.push(window.scrollY)
      if (this.vet.length == 2) {
        if (this.vet[1] > this.vet[0]) {
          // this.$refs.headerL.classList.add('headerRelative');
          this.$refs.headerL.classList = ['headerRelative']
          //console.log(this.$refs.headerL = ['headerRelative'])
        } else {
          // this.$refs.headerL.classList.add('headerRelative');
          // console.log('alto')
        }
        this.vet[0] = this.vet[1]
        this.vet.pop();
      }
    }
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
  background: #0a192f;
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
  border: 2px solid #00b4ff;
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
</style>
