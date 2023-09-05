<template>
    <div class="body">
        <header>
            <nav class="navbar">
                <ul>
                    <li><a href="/home">Home</a></li>
                    <li><a href="/about">About</a></li>
                    <li><a href="/review">Review</a></li>
                    <li><a href="/contact">Contact</a></li>
                </ul>
            </nav>
        </header>

        <div class="iframe-container">
            <iframe :src="iframeSrc" frameborder="0" allowfullscreen class="embedded-iframe"></iframe>
        </div><br><br><br>
        <div class="pay">
            <nuxt-link to="/payment" class="payt">Procced to Pay</nuxt-link><br><br>
        </div>
    </div>
</template>
  
<script setup>
const iframeSrc = 'https://docs.google.com/forms/d/e/1FAIpQLSeGn5SgXeKkpycivIDiaoDpnOfX5maTMmyZbL3nQxOi60I9Xw/viewform?embedded=true'; // Replace with your iframe source URL

</script>
  
<style scoped>
* {
    margin: 0;
    padding: 0;
    /* box-sizing: border-box; */
    /* border: 2px solid red; */


}


.body {
    font-family: Arial, sans-serif;
    /* background: url('~/staticc/beach1.jpg') no-repeat center center/cover; */
    background-color: white;
    height: 100vh;
    /* ... (other existing styles) */
    /* Remove any margin or padding from the .body element */
    margin: 0;
    padding: 0;
    /* width: 100vh; */
    /* margin: 0px; */
    /* margin: 0; */
    /* padding: 0px; */
    /* border: 2px solid red; */
    /* background-color: rgb(22, 59, 128); */
}


header {
    background-color: rgb(3, 34, 90);
    top: 0;
    /* position: sticky; */
    /* background: url('../page2/beach1.jpg') no-repeat center center/cover; */
    /* opacity: 0.5; */
}


.navbar {
    justify-content: center;
    padding: 10px 0;

    /* ... (other existing styles) */

    z-index: 1000;
    background-color: rgba(3, 34, 90, 0.9);
    /* Add a slight background color */
    /* z-index: 1; */
    /* text-align: center; */
    /* border: 2px solid red; */
}


ul {
    display: flex;
    z-index: 1000;
    list-style: none;
    margin-left: 31%;
    /* margin-top: 3%; */
    /* border: 2px solid red; */
}

li {
    margin: 25px 15px;
}

a {
    color: white;
    text-decoration: none;
    padding: 5px 15px;
}

a:hover {
    background-color: rgb(3, 3, 71);
    border-radius: 12px;
    color: white;
}

.a {
    color: white;
    text-decoration: none;
    padding: 5px 15px;
}

.head {
    font-size: 2em;
    text-align: center;
    margin: 2%;

}

.iframe-container {
    position: relative;
    top: 0%;
    left: 0;
    width: 100vw;
    background: white;
    /* 100% of viewport width */
    height: 80vh;
    /* 100% of viewport height */
    z-index: 9999;
    /* Adjust z-index as needed */
}

.embedded-iframe {
    width: 100%;
    height: 100%;
}

.pay {
    color: black;
    background: white;
    /* border: 2px solid red; */
    font-size: 1em;
    text-align: center;
    margin-top: 0%;
    margin-bottom: 0%;
}

.payt {
    color: white;
    padding: 6px 25px;
    /* color: white; */
    border: 2px solid black;
    background-color: rgba(3, 34, 90, 0.9);
    margin: 0%;
    font-size: 1.5rem;
    border-radius: 12px;
    font-family: 'Bree Serif', serif;
    cursor: pointer;
    text-decoration: none;
}



.payt:hover {
    /* transform: scale(1.2); */
    background-color: rgba(3, 34, 90, 0.9);
    color: white;
}
</style>
  