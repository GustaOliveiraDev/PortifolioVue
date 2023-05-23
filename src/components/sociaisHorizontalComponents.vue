<template>
  <div class="socialApresentacao q-gutter-xs">

    <div class="ApresentacaoIcon"><a  @click="enviarEmail" target="_blank">
      <q-icon size="xl" name="fa-solid fa-square-envelope" />
      </a>
    </div>

    <div class="ApresentacaoIcon"><a href="https://github.com/GustaOliveiraDev" target="_blank">
        <q-icon size="xl" name="fa-brands fa-square-github" />
      </a>
    </div>

    <div class="ApresentacaoIcon"><a href="https://www.instagram.com/gustvex/" target="_blank">
        <q-icon size="xl" name="fa-brands fa-square-instagram" />
      </a>
    </div>

    <div class="ApresentacaoIcon"><a href="https://www.linkedin.com/in/gustavo-oliveira-10383b231/" target="_blank">
        <q-icon size="xl" name="fa-brands fa-linkedin" />
      </a>
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
.socialApresentacao {
  display: flex;
  margin-top: 1em;
}

.ApresentacaoIcon a{
  color: white;
  text-decoration: none;
}


.ApresentacaoIcon a:hover {
  transition: 0.3s;
  color: #00b4ff;

}

</style>
