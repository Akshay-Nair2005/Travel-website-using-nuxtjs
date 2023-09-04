<template>
    <div class="body">
        <header>
            <nav class="navbar">
                <ul>
                    <li><a href="/home">Home</a></li>
                    <li><a href="/destination">Destination</a></li>
                    <li><a href="/review">Review</a></li>
                    <li><a href="/contact">Contact</a></li>
                </ul>
            </nav>
        </header>
        <div class="about-us-page">
            <section class="about-content">
                <h1>About Us</h1>
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
                    <img src="./static/c_c2.jpg" alt="Team Member 1" />
                    <h3>Akshay Nair</h3>
                    <p>Founder & CEO</p>
                </div>
                <div class="team-member">
                    <img src="./static/c_c2.jpg" alt="Team Member 2" />
                    <h3>Amir Chaus</h3>
                    <p>Travel Specialist</p>
                </div>
                <div class="team-member">
                    <img src="./static/c_c2.jpg" alt="Team Member 2" />
                    <h3>Aaditi Bhosale</h3>
                    <p>Travel Specialist</p>
                </div>
                <div class="team-member">
                    <img src="./static/c_c2.jpg" alt="Team Member 2" />
                    <h3>Aravind Gajula</h3>
                    <p>Travel Specialist</p>
                </div>
                <div class="team-member">
                    <img src="./static/c_c2.jpg" alt="Team Member 2" />
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
    max-width: 1200px;
    margin: 0 auto;
    padding: 20px;
}

.about-content {
    margin-bottom: 40px;
}

.team-members {
    display: flex;
    /* flex-direction: column; */
    align-items: center;
    margin-bottom: 20px;
    /* border: 2px solid black; */
    /* padding-left: 5%; */
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
    color: #777;
}

h1,
h2 {
    text-align: center;
    color: #333;
}

p {
    line-height: 1.6;
    color: #666;
}

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
</style>
  