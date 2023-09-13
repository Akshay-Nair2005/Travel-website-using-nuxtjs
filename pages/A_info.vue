<template>
    <div class="body"><br>
        <header>
            <nav>
                <h3><span>H</span>imachal Paradise</h3>
                <ul>
                    <li class="item"><nuxt-link to="/destination">Destination</nuxt-link></li>
                    <li class="item"><nuxt-link to="/about">About Us</nuxt-link></li>
                    <li class="item"><nuxt-link to="/contact">Contact</nuxt-link></li>
                    <li class="item"><nuxt-link to="/review">Review</nuxt-link></li>
                </ul>
                <i class="bi bi-three-dots"></i>
                <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-three-dots"
                    viewBox="0 0 16 16">
                    <path
                        d="M3 9.5a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3zm5 0a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3zm5 0a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3z" />
                </svg>
            </nav>
            <div class="content">
                <div class="cont">
                    <h2>Welcome to Himachal Pradesh</h2>
                    <p>Experience the breathtaking beauty of Himachal!</p>
                    <br>
                    <a href="https://en.wikipedia.org/wiki/Himachal_Pradesh" target="_blank">Explore Himachal</a>
                    <br><br><br>
                    <h3>Activities to Enjoy</h3>
                </div>
                <div class="cardholder">
                    <div class="card">
                        <img src="./static/kerala.jpg" alt="Himachal Pradesh">
                        <h4>Trekking Adventures</h4>
                        <p>Explore the majestic Himalayan trails!</p>
                    </div>
                    <div class="card">
                        <img src="./static/kerala.jpg" alt="Himachal Pradesh">
                        <h4>Snowy Retreats</h4>
                        <p>Enjoy the snowy landscapes and skiing!</p>
                    </div>
                    <div class="card">
                        <img src="./static/kerala.jpg" alt="Himachal Pradesh">
                        <h4>Cultural Festivals</h4>
                        <p>Participate in vibrant local festivals!</p>
                    </div>
                    <div class="card">
                        <img src="./static/kerala.jpg" alt="Himachal Pradesh">
                        <h4>Wildlife Exploration</h4>
                        <p>Discover the diverse wildlife of Himachal!</p>
                    </div>
                </div>
            </div>
        </header>
        <div class="whole">
            <div class="trip">
                <h3>Historical importance</h3>
                <div class="info">
                    <p class="para">
                        <!-- Your content goes here -->
                        Ancient Civilization: Kerala has a rich history dating back to ancient times, with evidence of human
                        settlements that date back to the Neolithic period.
                        Trade Routes: Due to its strategic location along the ancient maritime trade routes, Kerala
                        attracted traders
                        from various parts of the world, including the Greeks, Romans, Arabs, and Chinese.
                        Colonial Influences: Kerala witnessed the colonial rule of the Portuguese, Dutch, and British, each
                        leaving
                        their mark on the culture, architecture, and governance of the region.
                        Muziris: An ancient port city, Muziris was a thriving trade center that connected India with the
                        rest of the
                        world. Its ruins and artifacts provide insights into the region's historic significance.
                    </p>
                    <img class="k1_img" src="./static/kerala_bg.jpg" alt="random">
                </div>
            </div>
            <div class="trip">
                <h3>Cultural Performances</h3>
                <div class="info">
                    <p class="para">
                        <!-- Your content goes here -->
                        Art Forms: Kerala is renowned for its traditional art forms like Kathakali (classical dance-drama),
                        Mohiniyattam (classical dance), Theyyam (ritual dance), and Kalaripayattu (martial art).
                        Festivals: The state is known for its vibrant festivals such as Onam, Vishu, and Thrissur Pooram,
                        where grand
                        processions, traditional performances, and rituals take place.
                        Religious Diversity: Kerala is home to a diverse array of religious communities, including Hindus,
                        Christians,
                        Muslims, and Jews, contributing to a tapestry of religious festivals and practices.
                        Ayurveda and Wellness: The ancient science of Ayurveda originated in Kerala. Visitors can experience
                        traditional Ayurvedic treatments and therapies for holistic well-being.

                        <img class="k1_img" src="./static/kerala_bg.jpg" alt="random">
                    </p>
                </div>
            </div>
            <div class="trip">
                <h3>Cuisines</h3>
                <div class="info">
                    <p class="para">
                        <!-- Your content goes here -->
                        Coconut-based Dishes: Kerala's cuisine is known for its generous use of coconut in various forms -
                        grated,
                        coconut milk, and coconut oil - adding a distinct flavor to dishes.
                        Sadya: A traditional feast served on banana leaves, Sadya includes a variety of vegetarian dishes
                        and is a
                        staple during festivals like Onam.
                        Seafood Delicacies: With a long coastline, Kerala offers a wide range of seafood dishes such as
                        Karimeen
                        Pollichathu (pearl spot fish) and Meen Curry (fish curry).
                        Spices and Aromatics: The land of spices, Kerala's cuisine is rich with flavors like cardamom, black
                        pepper,
                        cinnamon, and cloves, enhancing the taste of dishes.
                        Appam and Stew: Appam, a rice pancake with a crispy edge, is often paired with vegetable or meat
                        stew,
                        offering a unique blend of textures and flavors.
                    </p>
                    <img class="k1_img" src="./static/kerala_bg.jpg" alt="random">
                </div>
                <br><br><br><br>
            </div>
            <br><br>
        </div>
        <div class="button">
            <!-- <a href="k_explore.vue" class="default">Book Available Packages</a> -->
            <nuxt-link to="/K_explore" class="a">Book Available Packages</nuxt-link>
            <a href="/Hotel1" class="a">Customize your own Package</a>
        </div>
        <footer class="foot">
            <div id="footer-top" class="social-footer">
                <div class="container">
                    <div class="region region-footer-top">
                        <div id="block-block-1" class="block block-block">
                            <div class="content">
                                <div class="col-md-12 sf-icons">
                                    <a href="#" target="_blank"> <span class="icon">
                                            <font-awesome-icon :icon="['fab', 'youtube']" /></span> </a>
                                    &nbsp;&nbsp;&nbsp;&nbsp;
                                    <a href="#" target="_blank"><span class="icon"><font-awesome-icon
                                                :icon="['fab', 'instagram']" /></span></a>
                                    &nbsp;&nbsp;&nbsp;&nbsp;
                                    <a href="#" target="_blank"><span class="icon"><font-awesome-icon
                                                :icon="['fab', 'twitter']" /></span></a>
                                    &nbsp;&nbsp;&nbsp;&nbsp;
                                    <a href="#" target="_blank"><span class="icon"><font-awesome-icon
                                                :icon="['fab', 'telegram']" /></span></a>
                                    &nbsp;&nbsp;&nbsp;&nbsp;
                                    <a href="#" target="_blank"><span class="icon"><font-awesome-icon
                                                :icon="['fab', 'facebook']" /></span></a>
                                    &nbsp;&nbsp;&nbsp;&nbsp;
                                </div>
                                <div class="row">
                                    <div class="col col-sm-12">
                                        <div class="foot">
                                            <p>&copy; 2012 Tourism Company. All rights reserved.</p>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </footer>

    </div>
</template>
  
<style scoped>
/* Your CSS styles here */
* {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    /* background-color: #c1f5d0; */
}

.body {
    font-family: 'Poppins', sans-serif;
    z-index: 10;
    /* background: url('~/staticc/nature4.jpg') no-repeat center center/cover; */
    background-color: #c3e6e6;
    /* font-family: 'Roboto', sans-serif; */
    /* border: 1px solid red; */
}

header {
    width: 80%;
    height: 95vh;
    /* border: 2px solid red; */
    margin: auto;
}

header nav {
    width: 95%;
    height: 7%;
    /* border: 2px solid red; */
    margin: auto;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

header nav h3 {
    color: #006666;
    /* Teal text color */
}

header nav h3 span {
    color: black;
}

header nav ul {
    list-style: none;
    display: flex;

}

header nav ul li {
    padding: 3px 15px;

}

header nav ul li:nth-last-child(1) {
    background: #014917;
    border-radius: 20px;
    padding: 5px 20px;
    background: #006666;
}

header nav ul li:nth-last-child(1):hover {
    background: rgb(30, 155, 30);
    background: #009999;
}

header nav ul li:nth-last-child(1) a:hover {
    color: black;
    color: white;
}

header nav ul li:nth-last-child(1) a {
    color: white;
    /* color: #006666; */
}

header nav ul li a {
    text-decoration: none;
    color: #009999;
    font-size: 17px;
    font-weight: bold;
    transition: .3s linear;
}


header nav ul li a:hover {
    color: white;

}

header nav .bi-three-dots {
    display: none;
}

header .content {
    position: relative;
    height: 80%;
    width: 100%;
    z-index: 20;
    /* border: 2px solid red; */
}

header .content::before {
    content: '';
    /* position: absolute; */
    position: absolute;
    width: 100%;
    height: 80%;
    border-radius: 10px;
    background-color: #014917;
    background: url("~/staticc/kerala_bg.jpg")no-repeat center center/cover;
    /* z-index: -1; */

    /* border: 2px solid red; */
}

.cont {
    position: absolute;
    width: 700px;
    height: auto;
    color: #d8fcd8;
    padding: 30px;
    z-index: 30;
    font-size: 16px;
    /* z-index: 9; */
}

header .content .cont h2 {
    line-height: 40px;
    font-weight: 800;
    /* margin: 0; */
    /* border: 1px solid red; */
}

header .content .cont p {
    font-size: 15px;
    font-weight: 800;
    padding-top: 10px;
}

header .content .cont a {
    margin-top: 30px;
    padding: 8px 20px;
    border-radius: 20px;
    border: 2px solid #006666;
    background: #006666;
    color: white;
    outline: none;
    cursor: pointer;
    transition: .3s linear;
    text-decoration: none;
    font-size: 17px;
    font-weight: bold;

}

header .content .cont a:hover {
    background: green;
    border: 1px solid green;
}


.cardholder {
    display: flex;
    position: absolute;
    margin-top: 25%;

}

.card {
    /* position: relative; */
    display: block;
    width: 22%;
    /* background-color: rgb(7, 126, 21); */
    /* margin-top: 25%; */
    background-color: green;
    border-radius: 25%;
    padding: 30px 20px;
    margin: 0px 20px;
    box-shadow: 0px 0px 10px rgb(10, 78, 16);
    border: 2px solid white;
    color: white;
    opacity: 0.9;
    background-color: #009999;
    /* Cyan card background */
    box-shadow: 0px 0px 10px #009999;
    /* Cyan card shadow */
    /* background-color: #054708; */
    /* border: 2px solid rgb(3, 46, 10); */
    /* color: black; */
    /* z-index: 10; */
    /* border: 2px solid rgb(31, 139, 44); */
    /* background: url('../page2/beach.jpg') no-repeat center center/cover; */
    /* box-shadow: 0px 0px 5px rgba(0, 0, 0, 0.2); */
    /* z-index: 50000; */
}

.card:hover {
    transform: scale(1.1);
}

.card img {
    width: 100%;
    height: 100px;
    object-fit: cover;
    border-radius: 25%;
    margin-bottom: 10px;
    border: 2px solid rgb(3, 46, 10);
    box-shadow: 0px 0px 40px rgb(167, 224, 167);
    z-index: 2;
    border: 2px solid white;
}

.card h4 {
    font-size: 17px;
    margin-bottom: 0px;
    font-weight: bold;
    text-align: center;
    text-decoration: underline;
    z-index: 2;
    padding-top: 15px;
}


.card p {
    font-size: 20px;
    margin-bottom: 0px;
    /* font-weight: bold; */
    padding-top: 15px;
    text-align: center;
    z-index: 2;
    /* color: #006666; */
}

.whole {
    display: block;
    margin-left: 5%;
    margin-top: 2%;
    width: 90%;
    border: 2px solid lightgreen;
    border-radius: 7%;
    box-shadow: 0px 0px 20px rgb(126, 190, 126);
    background-color: #054708;
    background-color: #009999;
    background-image: linear-gradient(to right, #009999, #baf8f8);
    /* Cyan background */
    border: 2px solid white;
    /* Cyan border */
    box-shadow: 0px 0px 20px white;
    /* Cyan shadow */
}

.trip {
    position: relative;
    width: 95%;
    height: auto;
    margin-left: 7%;
    margin-top: 5%;
    /* text-align: center; */
    color: white;
    /* border: 1px solid green; */
}

.trip h3 {
    font-size: 20px;
    text-shadow: 0px 0px 10px #009999;
    /* Cyan text shadow */
    /* color: #006666; */
    /* Teal text color */
}

.trip .info {
    display: flex;
    margin-top: 3%;
    text-align: left;
    /* padding-left: 60%; */
    /* margin-left: 10%; */
}

.trip .info .para {
    display: flex;
    width: 50%;
    text-shadow: 0px 0px 10px lightgreen;
    font-size: 1.2rem;
    /* border: 1px solid red; */
    /* margin-left: 10%; */
    text-shadow: 0px 0px 10px #009999;
    /* Cyan text shadow */
    font-size: 1.2rem;
    /* color: #006666; */
    /* Teal text color */
}

.trip .info img {
    position: absolute;
    right: 5%;
    width: 40%;
    border: 2px solid lightgreen;
    border-radius: 20px;
    box-shadow: 0px 0px 20px lightgreen;
    border: 2px solid white;
    /* Cyan border around images */
    box-shadow: 0px 0px 20px #009999;
    /* Cyan image shadow */
    /* margin-left: 60%; */
}

.trip .info img:hover {
    transform: scale(1.07);
}

.button {
    margin-top: 5%;
    display: flex;
}

.button .a {
    width: 44%;
    margin-left: 5%;
    margin-top: 30px;
    padding: 10px 20px;
    border-radius: 10px;
    border: 2px solid rgb(1, 26, 4);
    background: rgb(1, 26, 4);
    color: white;
    outline: none;
    cursor: pointer;
    text-align: center;
    text-decoration: none;
    font-size: 13px;
    font-weight: bold;
    background: #006666;
    /* Teal background */
    border: 2px solid white;
    /* Teal border */
    color: white;
    /* transition: .3s linear; */

}

.button .a:hover {
    background: #009999;
    /* Cyan background on hover */
    border: 2px solid #009999;
    /* Cyan border on hover */
}

footer {
    background-color: #023304;
    color: #fff;
    margin-top: 6.35%;
    padding: 20px;
    text-align: center;
    width: 100%;
    background-color: #006666;
    /* Teal footer background */
    color: white;
    /* opacity: 0.6; */
    /* z-index: ; */
    /* border: 2px solid green; */

}

.row {
    text-align: center;
}
</style>
  
  <!-- <script>
  export default {
    name: 'KeralaInfo',
    // Any JavaScript functionality goes here
  }
  
  </script> -->
  
  