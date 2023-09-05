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
        <div class="about-us-page">
            <section class="about-content">
                <h1>About Us</h1><br>
                <p>Welcome to Travelopedia, your trusted partner for unforgettable travel experiences.</p>
                <p>We are a passionate team of travel enthusiasts dedicated to creating memorable journeys that cater to all
                    kinds of travelers. Whether you're an adventure seeker, a culture explorer, or a relaxation lover, we
                    have
                    something special for everyone.</p>
                <p>Our mission is to provide you with seamless travel experiences, from the moment you dream about your trip
                    to
                    the moment you return home with a heart full of memories. We handpick the best destinations,
                    accommodations,
                    and activities to ensure you have a truly immersive and enjoyable experience.</p>
                <p>Join us on a journey that goes beyond the ordinary, and let's explore the world together.</p>
            </section>
            <h2>Meet Our Team</h2>
            <br><br>
            <section class="team-members">
                <div class="team-member">
                    <img src="./static/c_c4.jpg" alt="Team Member 1" />
                    <h3>Akshay Nair</h3>
                    <p>Founder & CEO</p>
                </div>
                <div class="team-member">
                    <img src="./static/c_c4.jpg" alt="Team Member 2" />
                    <h3>Amir Chaus</h3>
                    <p>Travel Specialist</p>
                </div>
                <div class="team-member">
                    <img src="./static/c_c4.jpg" alt="Team Member 2" />
                    <h3>Aaditi Bhosale</h3>
                    <p>Travel Specialist</p>
                </div>
                <div class="team-member">
                    <img src="./static/c_c4.jpg" alt="Team Member 2" />
                    <h3>Aravind Gajula</h3>
                    <p>Travel Specialist</p>
                </div>
                <div class="team-member">
                    <img src="./static/c_c4.jpg" alt="Team Member 2" />
                    <h3>Sanika Warange</h3>
                    <p>Travel Specialist</p>
                </div>
                <!-- Add more team members as needed -->
            </section>
        </div>
    </div>
</template>
  
<style scoped>
.about-us-page {
    /* position: absolute; */
    max-width: 1200px;
    margin: 0% auto;
    padding: 20px;
    background: black;
    box-shadow: 0px 0px 15px white;
    border-radius: 15px;
    /* border: 2px solid white; */
    opacity: 0.85;
    z-index: 0;

}

.about-content {
    margin-bottom: 40px;
    z-index: 10;

}

.team-members {
    display: flex;
    /* flex-direction: column; */
    align-items: center;
    margin-bottom: 20px;
    /* border: 2px solid black; */
    /* padding-left: 5%; */
    /* z-index: 1000000; */
}

.team-member {
    display: block;
    margin-left: 5%;
}

.team-members img {
    width: 150px;
    height: 150px;
    border-radius: 50%;
    margin-bottom: 10px;
}

.team-members h3 {
    margin: 0;
}

.team-members p {
    font-style: italic;
    color: white;
}

h1,
h2 {
    text-align: center;
    color: white;
}

p {
    line-height: 1.6;
    color: white;
}

* {
    margin: 0;
    padding: 0;
    /* box-sizing: border-box; */
    /* border: 2px solid red; */


}


.body {
    font-family: Arial, sans-serif;
    height: 100vh;
    /* ... (other existing styles) */
    /* Remove any margin or padding from the .body element */
    margin: 0;
    padding: 0;
    color: white;
    z-index: -1;
    /* width: 100vh; */
    /* margin: 0px; */
    /* margin: 0; */
    /* padding: 0px; */
    /* border: 2px solid red; */
    /* background-color: rgb(22, 59, 128); */
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
    margin-top: 1.5%;
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
    margin-top: 1.5%;
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
</style>
  