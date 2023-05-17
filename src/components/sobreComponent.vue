<template>
  <div class="  conteudoSobre">

    <div class=" text-normal">
      conteudoSobre
    </div>
    <div class="text-titulo">
      Brittany Chiang.
      I build things for the web.
    </div>

    <div class=" text-normal">
      a software engineer specializing in building (and occasionally designing)
      exceptional digital experiences. Currently, Im focused on building accessible,
      human-centered products at Upstatement.
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
.conteudoSobre {
  margin-top: 10vh;
  margin-bottom: 50vh;
  align-items: start;
  width: 50vw;
  /* border: 1px solid red; */
}
.text-titulo{
  font-size: clamp(36px, 36px + 36px, 36px);
  color: white;
}
.text-normal{
  font-size: clamp(16px, 16px + 16px, 16px);
  color: #00b4ff;
}
</style>