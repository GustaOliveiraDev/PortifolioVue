<template>
    <div class="containerSocialEmail">

        <div class="socialEmail">

            <div round class="socialTexEmail">
                GustaOliveiraDev@gmail.com
            </div>

        </div>

        <div class="socialLineEmail">
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
.containerSocialEmail {
    position: fixed;
    right: 50px;
    bottom: 0px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}

.socialEmail {
    height: 150px;
    color: white;
}

.socialTexEmail {
    display: flex;
    justify-content: center;
    align-items: center;
    transform: rotate(90deg);
    width: 30px;
}

.socialTexEmail:hover {
    transition-duration: 0.3s;
    color: #00b4ff;
    padding-right: 10px;
}

.socialLineEmail {
    border-right: 1px solid;
    height: 200px;
    color: white;
}

@media (max-width: 600px) {

    .containerSocialEmail {
        display: none;
    }

    /* .socialLineEmail {
    border-right: 1px solid;
    height: 200px;
    color: #00b4ff;
}
.socialEmail {
    height: 150px;
    color: #00b4ff;
} */

}
</style>