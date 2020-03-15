<template>
<div class="camera">
<video autoplay></video>
<button>SNAP</button>
</div>
</template>

<script>
export default {
    name: 'camera'
}
</script>

<style scoped>
.camera {
    width: 100%;
    height: 100vh;
    padding: 25px;
    box-sizing: border-box;
}
.feed {
    width: 100%;
    max-width: 1280px;
    margin: 0 auto;
    background-color: #171717;
    box-shadow: 6px 6px 12px 0px rgba(0,0,0,0.25);
}
.snap {

}
</style>