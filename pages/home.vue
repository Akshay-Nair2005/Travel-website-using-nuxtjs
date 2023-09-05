<template>
    <div class="body">
        <header class="header">
            <nav class="navcontainer">
                <a href="#"><span>T</span>ravelopedia</a>
            </nav>
            <nav class="navbar">
                <ul>
                    <li class="item"><nuxt-link to="/destination">Destination</nuxt-link></li>
                    <li class="item"><nuxt-link to="/about">About</nuxt-link></li>
                    <li class="item"><nuxt-link to="/review">Review</nuxt-link></li>
                    <li class="item"><nuxt-link to="/contact">Contact</nuxt-link></li>
                    <li class="item"><nuxt-link to="/present">Presentation</nuxt-link></li>
                </ul>
            </nav>
        </header>
        <div class="whole">
            <div class="container">
                <h1>Welcome to Travelopedia</h1><br>
                <h3>Explore the World</h3><br>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Vel perferendis</p><br><br>
                <nuxt-link to="/destination" class="explore">Start Your Journey</nuxt-link>
            </div>

            <div class="carousel-container">
                <div class="carousel">
                    <img src="./static/nature5.jpg" alt="Image 1">
                    <img src="./static/nature6.jpg" alt="Image 2">
                    <img src="./static/nature3.jpg" alt="Image 3">
                    <img src="./static/nature4.jpg" alt="Image 4">
                    <img src="./static/nature7.jpg" alt="Image 5">
                    <img src="./static/nature8.jpg" alt="Image 6">
                </div>
            </div>
        </div>
    </div>
</template>
  
<style>
/* Your CSS styles go here */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    font-size: 1em;
    color: rgb(165, 165, 165);
    background: url('~/staticc/nature4.jpg') no-repeat center center/cover;
    /* Replace 'background.jpg' with your actual background image path */
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    background-attachment: fixed;
    /* opacity: 0.85; */
}

.header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
}

.navcontainer {
    font-size: 1.5em;
    color: white;
    text-decoration: none;
    margin-top: 3.5%;
    margin-left: 5%;
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
}

.navcontainer a {
    font-size: 1.3em;
    color: white;
    text-decoration: none;
    margin-left: 3%;
}

.navcontainer span {
    font-size: 1.5em;
    color: orange;

}



.navbar {
    /* border: 2px solid white; */
    margin-top: 3.5%;
    margin-right: 15%;
}

.navbar ul {
    list-style: none;
    display: flex;
}

.navbar li {
    margin-right: 15%;
    /* border: 2px solid red; */
    /* padding-right: 3%; */
}

.navbar a {
    text-decoration: none;
    color: white;
    /* transition: all .5s; */
}

.navbar a:hover {
    text-decoration: underline;
    /* color: white; */
}

.container {
    text-align: left;
    padding: 7%;
    margin-top: 1.6%;
    color: white;
}

.container a {
    text-decoration: none;
}

.explore {
    margin-top: 1.5%;
    font-size: 1.2em;
    background-color: transperant;
    border: 2px solid orange;
    color: white;
    padding: 10px 20px;
    border-radius: 5px;
    width: 40%;
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
}

h1,
h3,
p {
    padding-top: 0.8%;
}

.dest {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
}

.img {
    margin: 20px;
    border: 2px solid white;
}

.img img {
    width: 200px;
    /* Adjust as needed */
    height: 150px;
    /* Adjust as needed */
}

.carousel-container {
    margin-top: 10%;
    margin-left: 20%;
    width: 250px;
    height: 150px;
    perspective: 800px;
}

.carousel {
    width: 100%;
    height: 100%;
    position: relative;
    transform-style: preserve-3d;
    animation: rotateCarousel 10s infinite linear;
}

.carousel img {
    width: 100%;
    height: 100%;
    position: absolute;
    transform-origin: center;
    transition: transform 2s;
    border-radius: 5%;
    border: 2px solid white;
    box-shadow: 0 0 20px orange;
}

.carousel img :hover {
    transform: scale(1.2);
    box-shadow: 0 0 10px black;
}

.carousel img:nth-child(1) {
    transform: rotateY(0deg) translateZ(280px);
}

.carousel img:nth-child(2) {
    transform: rotateY(60deg) translateZ(280px);
}

.carousel img:nth-child(3) {
    transform: rotateY(120deg) translateZ(280px);
}

.carousel img:nth-child(4) {
    transform: rotateY(180deg) translateZ(280px);
}

.carousel img:nth-child(5) {
    transform: rotateY(240deg) translateZ(280px);
}

.carousel img:nth-child(6) {
    transform: rotateY(300deg) translateZ(280px);
}


@keyframes rotateCarousel {
    0% {
        transform: rotateY(0deg);
    }

    100% {
        transform: rotateY(360deg);
    }
}

.whole {
    display: flex;
}
</style>
  