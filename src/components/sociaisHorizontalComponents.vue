<template>
    <div class="socialApresentacao q-gutter-xs">

        <div class="ApresentacaoIcon">
            <q-icon size="xl" name="fa-brands fa-square-github" />
        </div>

        <div class="ApresentacaoIcon">
            <q-icon size="xl" name="fa-brands fa-square-instagram" />
        </div>

        <div class="ApresentacaoIcon">
            <q-icon size="xl" name="fa-solid fa-square-envelope" />
        </div>

        <div class="ApresentacaoIcon">
            <q-icon size="xl" name="fa-brands fa-linkedin" />
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

.ApresentacaoIcon {
    color: white;
}


.ApresentacaoIcon:hover {
    transition: 0.3s;
    color: #00b4ff;

}
</style>