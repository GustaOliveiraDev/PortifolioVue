<template>
    <transition class="pai-loadig">
        <transition name="fade">
            <div v-if="show" class="i">
                <img v-if="show" class="imgLoader" src="../../public/imgs/AdobeStock_550513538_Preview.png">

            </div>
        </transition>
    </transition>
</template>

<script>
export default {
    data() {
        return {
            show: true,
        };
    },

    mounted() {
        this.showToggle()
    },
    methods: {
        showToggle() {
            setTimeout(() => {
                this.show = false
            }, 1000)
        }
    }

}
</script>

<style>
.pai-loadig {
    width: 100vw;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
   
}

.imgLoader {
    width: 400px;
    height: 400px;
    border-radius: 50%;
    /* background-color: #00b4ff; */
    background-color: #0a192f;
}

.i{
    width: 100vw;
    height: 100vh;
    background-color: #0a192f;

    /* background-color: #00b4ff; */
}

.fade-enter-active,
.fade-leave-active {
    transition: 1s;
}

.fade-enter,
.fade-leave-to {

    
    opacity: 0;
}


</style>