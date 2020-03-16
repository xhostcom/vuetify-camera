<template>
<section class="top" justify-center align-center>
         <div class="mb-12 camera">
         <video autoplay class="feed"></video>
         <br />
         <v-btn block dark color="info">SNAP</v-btn>
        </div>
</section>
</template>
<script>
export default {
    name: 'Camera',
    methods: {
      init () {
        if('mediaDevices' in navigator && 'getUsermedia' in navigator.mediaDevices) {
            navigator.mediaDevices.getUserMedia[{video: true}]
            .then(stream => {
                 const videoPlayer = document.querySelector('video')
                 videoPlayer.srcObject = stream;
                 videoPlayer.play;
            });
        } else {
            alert('Cannot get media Devices');
        }
      }
    },
    beforeMount () {
        this.init();
    }
}
</script>
<style lang = "scss" scoped>
.camera {
    width: 100vw;
    height: 100vh;
    padding: 25px;
    box-sizing: border-box;
}
.feed {
    display: block;
    width: 100%;
    max-width: 1280px;
    margin: 0 auto;
    background-color: #171717;
    box-shadow: 6px 6px 12px 0px rgba(0,0,0,0.35);
}
.snap {
    display: block;
    width: 75px;
    height: 75px;
    border-radius: 50%;
    margin: 25 auto;
    background-color: transparentize($color: #ffce00, $amount: 0.5);
    border: solid 1px #171717;
    outline: none;

    cursor: pointer;

    &:hover {
        background-color: #ffce00;
    }
    &:active {
        background-color: #ffce00;
    }
}
</style>
