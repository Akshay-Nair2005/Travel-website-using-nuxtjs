<template>
    <div class="iframe-container">
        <iframe :src="iframeSrc" frameborder="0" allowfullscreen class="embedded-iframe"></iframe>
    </div>
</template>
  
<script setup>
const iframeSrc = 'https://gamma.app/embed/csrc7jtt1yaiv1l'; // Replace with your iframe source URL
</script>
  
<style scoped>
.iframe-container {
    position: fixed;
    top: 0;
    left: 0;
    width: 100vw;
    /* 100% of viewport width */
    height: 100vh;
    /* 100% of viewport height */
    z-index: 9999;
    /* Adjust z-index as needed */
}

.embedded-iframe {
    width: 100%;
    height: 100%;
}
</style>
  