<template>
  <div class="containerSocial">

    <div class="socialMidia">

      <div class="socialIcon">
        <q-btn flat round dense icon="fa-brands fa-square-github" />
      </div>
      <div class="socialIcon">
        <q-btn flat round dense icon="fa-brands fa-square-instagram" />
      </div>
      <div class="socialIcon">
        <q-btn flat round dense icon="fa-brands fa-linkedin" />
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

}
</script>

<style>
.containerSocial {
  position: fixed;
  left: 50px;
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

.socialLine {
  border-right: 1px solid;
  height: 200px;
  color: white;
}

.socialIcon:hover {
  transition: 0.3s;
  padding-bottom: 10px;
  color: #00b4ff;

}

@media (max-width: 600px) {

  /* .socialLine {
    color: #00b4ff;
  }

  .socialMidia {
    color: #00b4ff;
  } */

  .containerSocial {
display: none;
}

}
</style>