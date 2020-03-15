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
    data () {
  }
}
</script>
<style scoped>
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
    box-shadow: 6px 6px 12px 0px rgba(0,0,0,0.25);
}
</style>
