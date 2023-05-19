<template>
  <div class="socialApresentacao q-gutter-xs">

    <div class="ApresentacaoIcon"><a href="https://github.com/GustaOliveiraDev" target="_blank">
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

    <div class="ApresentacaoIcon"><a href="www.linkedin.com/in/gustavooliveiradevv" target="_blank">
        <q-icon size="xl" name="fa-brands fa-linkedin" />
      </a>
    </div>

  </div>
</template>

<script>
export default {

}
</script>

<style>
.socialApresentacao {
  display: flex;
  margin-top: 1em;
}

.ApresentacaoIcon a{
  color: white;
}


.ApresentacaoIcon a:hover {
  transition: 0.3s;
  color: #00b4ff;

}

</style>
