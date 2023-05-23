<template>
  <div class="containerSocial">

    <div class="socialMidia">

      <div class="socialIcon"><a @click="enviarEmail" target="_blank">
      <q-icon size="sm" name="fa-solid fa-square-envelope" />
      </a>
    </div>

    <div class="socialIcon"><a href="https://github.com/GustaOliveiraDev" target="_blank">
        <q-icon size="sm" name="fa-brands fa-square-github" />
      </a>
    </div>

    <div class="socialIcon"><a href="https://www.instagram.com/gustvex/" target="_blank">
        <q-icon size="sm" name="fa-brands fa-square-instagram" />
      </a>
    </div>

    <div class="socialIcon"><a href="https://www.linkedin.com/in/gustavo-oliveira-10383b231/" target="_blank">
        <q-icon size="sm" name="fa-brands fa-linkedin" />
      </a>
    </div>
    </div>

    <div class="socialLine">
      <div>

      </div>
    </div>

  </div>
</template>

<script>
export default {
  methods: {
        enviarEmail() {
            window.location.href = `mailto:?body=Olá, entrei no endereço  e econtrei a norma
              nº  - MT, gostaria de compartilha-la com você, para acessá-lá clique no link: `;
        },
    }
}
</script>

<style>
.containerSocial {
  position: fixed;
  left: 25px;
  bottom: 0px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

.socialMidia {
  color: white;
}

.socialIcon {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 10px;
  width: 30px;
  height: 30px;
}

.socialIcon a {
text-decoration: none;
color: white;
}

.socialLine {
  border-right: 1px solid;
  transition: 0.3s;
  height: 200px;
  color: white;
}

.socialIcon a:hover {
  transition: 0.3s;
  padding-bottom: 10px;
  color: #00b4ff;

}

@media (max-width: 600px) {

  .containerSocial {
    display: none;
  }

}
</style>
