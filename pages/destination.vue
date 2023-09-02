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
        <div class="container">
            <div class="section1">
                <h2>From greenery to sand... From Oceans to land</h2>
                <h2>Explore the Options</h2>
                <br>
                <p>Plan your dream vacation with us</p>
            </div>
            <br>
            <h2 class="type">International</h2>
            <br><br>
            <div class="section">
                <div class="card">
                    <img src="./static/Dubai.jpg" alt="Dubai">
                    <h3>Dubai</h3><br><br>
                    <p>Who says, "Money cannot buy happiness!!!"</p>
                    <p>"Habibi, Welcome to Dubai!!!!"</p>
                    <!-- <a href="#">Explore</a> -->
                    <nuxt-link to="/D_info" class="a">Explore</nuxt-link>
                </div>
                <div class="card">
                    <img src="./static/Singapore.jpg" alt="Singapore">
                    <h3>Singapore</h3><br><br>
                    <p>"Where culture meets development!!".</p>
                    <!-- <a href="#">Explore</a> -->
                    <nuxt-link to="/S_info" class="a">Explore</nuxt-link>
                </div>
                <div class="card">
                    <img src="./static/london.webp" alt="London">
                    <h3>London</h3><br><br>
                    <p>Timeless Majesty and Modern Marvels!!</p>
                    <!-- <a href="#">Explore</a> -->
                    <nuxt-link to="/L_info" class="a">Explore</nuxt-link>
                </div>
            </div>
            <h2 class="type">Domestic</h2>
            <div class="section">
                <div class="card">
                    <img src="./static/kerala.jpg" alt="Kerala">
                    <h3>Kerala</h3><br><br>
                    <p>God's Own Country</p>
                    <p>"Habibi, Welcome to Ponani!!!!"</p>
                    <!-- <a href="/K_info">Explore</a> -->
                    <nuxt-link to="/K_info" class="a">Explore</nuxt-link>
                </div>
                <div class="card">
                    <img src="./static/Goa.jpg" alt="Goa">
                    <h3>Goa</h3><br><br>
                    <p>"Sun, Sand, Serenity!!".</p>
                    <!-- <a href="#">Explore</a> -->
                    <nuxt-link to="/G_info" class="a">Explore</nuxt-link>
                </div>
                <div class="card">
                    <img src="./static/himachal_pradesh.png" alt="Himachal Pradesh">
                    <h3>Himachal Pradesh</h3><br><br>
                    <p>Majestic Mountains and Enchanting Valleys!!</p>
                    <!-- <a href="#">Explore</a> -->
                    <nuxt-link to="/A_info" class="a">Explore</nuxt-link>
                </div>
            </div>
            <br><br>
        </div>
    </div>
</template>
  
<style scoped>
/* Copy the CSS styles from the <style> tag in the original code */

* {
    margin: 0;
    padding: 0;
    /* box-sizing: border-box; */
    /* border: 2px solid red; */


}


.body {
    font-family: Arial, sans-serif;
    background: url('~/staticc/beach1.jpg') no-repeat center center/cover;
    /* background-color: white; */
    height: 100%;
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
    position: sticky;
    top: 0;
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
    border-radius: 5px;
    color: white;
}

.a {
    color: white;
    text-decoration: none;
    padding: 5px 15px;
}



.container {
    margin-bottom: 0px;
    background-color: transparent;
    color: azure;
    opacity: 0.95;
    /* z-index: -1; */
    /* border: 2px solid red; */
    /* background: url('../beach.jpg') no-repeat center center/cover; */
    /* background-color: rgb(186, 250, 250); */
    /* box-shadow: 0px 0px 7px aquamarine; */
    /* background: #000; */
}


.section {

    padding: 20px 20px;
    margin-bottom: 0;
    background-color: transparent;
    display: flex;

}

.section1 {
    text-align: center;
    font-family: Arial, Helvetica, sans-serif;
    /* font-family: 'Pacifico', cursive; */
    color: azure;
    opacity: 0.8;
    margin-top: 5%;
    /* border: 2px solid red; */
}

h2 {
    font-size: 32px;
    padding-top: 15px;
    margin-top: 10px;
    margin-bottom: 10px;
    /* opacity: 1; */
    /* font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif; */
}

p {
    font-weight: bold;
    /* opacity: 1; */
}

.type {
    font-size: 24px;
    font-family: 'Pacifico', cursive;
    text-align: center;
    /* font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif; */
    /* font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif; */
}

.card {
    display: block;
    width: 25%;
    background: url('~/staticc/beach.jpg') no-repeat center center/cover;
    /* background-color: rgb(3, 34, 90); */
    border-radius: 5px;
    padding: 20px 20px;
    margin: 0px 20px;
    box-shadow: 0px 0px 30px rgb(8, 8, 8);
    border: 2px solid black;
    color: black;
    /* box-shadow: 0px 0px 5px rgba(0, 0, 0, 0.2); */
    /* background-color: transparent; */
    /* z-index: 50000; */
}

.card:hover {
    transform: scale(1.1);
}

.card img {
    width: 100%;
    height: 200px;
    object-fit: cover;
    border-radius: 5px;
    margin-bottom: 10px;
    border: 2px solid black;
}

.card h3 {
    font-size: 18px;
    margin-bottom: 5px;
    font-weight: bold;
    text-align: center;
    text-decoration: underline;
}

.card p {
    margin-bottom: 10px;
    font-weight: bold;
    text-align: center;
}

.card a {
    display: inline-block;
    background-color: transparent;
    color: black;
    font-weight: bold;
    padding: 10px 20px;
    text-decoration: none;
    border-radius: 5px;
    margin-top: 45px;
    border: 2px solid black;
    margin-left: 13%;
    width: 50%;
    text-align: center;
}

footer {
    background-color: rgb(53, 75, 116);
    margin-bottom: 0;
}

@media screen and (max-width: 768px) {
    .section {
        flex-direction: column;
        align-items: center;
    }

    .card {
        width: 80%;
        margin: 20px;
    }
}
</style>
  