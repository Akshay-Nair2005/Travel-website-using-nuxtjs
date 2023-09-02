<template>
    <div class="body">
        <header>
            <nav>
                <h3><span>T</span>ravelopedia</h3>
                <ul>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">About Us</a></li>
                    <li><a href="#">Services</a></li>
                    <li><a href="#">Contact</a></li>
                    <li><a href="#">Register</a></li>
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
                    <h2>Lorem ipsum dolor sit amet consectetur adipisicing elit. Deserunt, mollitia.</h2>
                    <p>Lorem ipsum dolor sit, amet consectetur adipisicing.</p>
                    <br>
                    <a href="https://en.wikipedia.org/wiki/Kerala" target="_blank">Know Goa More</a>
                    <br><br>
                    <h3>Activites to do!!! </h3>
                </div>
                <div class="cardholder">
                    <div class="card">
                        <img src="./static/kerala.jpg" alt="Kerala">
                        <h4>Backwater Cruises</h4>
                        <p>"Habibi, Welcome to Ponani!!!!"</p>
                    </div>
                    <div class="card">
                        <img src="./static/kerala.jpg" alt="Kerala">
                        <h4>Beach Relaxation</h4>
                        <p>"Habibi, Welcome to Ponani!!!!"</p>
                    </div>
                    <div class="card">
                        <img src="./static/kerala.jpg" alt="Kerala">
                        <h4>Wildlife Safaris</h4>
                        <p>"Habibi, Welcome to Ponani!!!!"</p>
                    </div>
                    <div class="card">
                        <img src="./static/kerala.jpg" alt="Kerala">
                        <h4>Cultural Performances</h4>
                        <p>"Habibi, Welcome to Ponani!!!!"</p>
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
                        Colonial Legacy: Goa's history is deeply intertwined with colonial powers like the Portuguese, who
                        ruled for nearly 450 years. This influence is visible in architecture, religion, and culture.
                        Portuguese Architecture: The state showcases a mix of architectural styles, with colonial-era
                        churches, cathedrals, and forts such as Basilica of Bom Jesus and Aguada Fort.
                        Old Goa: Known as the "Rome of the East," Old Goa was the capital during the Portuguese rule, and it
                        houses historical sites like Sé Cathedral and St. Augustine Tower.
                        Indo-Portuguese Culture: The fusion of Indian and Portuguese cultures has led to a unique blend in
                        Goan art, music, dance, and even in everyday life.
                        Freedom Struggle: Goa played a significant role in India's struggle for freedom from colonial rule,
                        and the state was liberated in 1961.

                    </p>
                    <img class="k1_img" src="./static/kerala_bg.jpg" alt="random">
                </div>
            </div>
            <div class="trip">
                <h3>Cultural Performances</h3>
                <div class="info">
                    <p class="para">
                        <!-- Your content goes here -->
                        Carnival and Festivals: Goa is famous for its vibrant Carnival, marked by parades, music, dance, and
                        colorful floats. Religious festivals like Christmas and Easter are also celebrated with fervor.
                        Music and Dance: Traditional Goan music genres like Fado and Dekhnni, coupled with folk dances like
                        Fugdi and Dhalo, contribute to the state's rich cultural tapestry.
                        Cuisine and Feni: Goan cuisine is a reflection of its diverse heritage, with seafood being a
                        highlight. Don't miss trying local dishes like Vindaloo, Xacuti, and Bebinca. Feni, a local liquor,
                        is also part of the culture.
                        Arts and Crafts: The state has a thriving artistic community, known for its pottery, terracotta,
                        azulejos (ceramic tiles), and handicrafts that reflect the local aesthetics.


                        <img class="k1_img" src="./static/kerala_bg.jpg" alt="random">
                    </p>
                </div>
            </div>
            <div class="trip">
                <h3>Cuisines</h3>
                <div class="info">
                    <p class="para">
                        <!-- Your content goes here -->
                        Spices and Flavors: Goan cuisine is known for its use of spices, particularly red chilies, giving
                        dishes a distinct flavor. The tangy and spicy Vindaloo is a prime example.
                        Bebinca and Sannas: Bebinca, a traditional Goan dessert made with layers of coconut milk and
                        jaggery, is a must-try. Sannas, steamed rice cakes, often accompany spicy curries.
                        Sorpotel and Choriz: Sorpotel is a popular pork dish with a spicy, tangy taste. Choriz, spicy
                        sausages, are a legacy of the Portuguese influence.
                        Feni: This cashew-based alcoholic drink comes in two varieties cashew apple feni and coconut feni.
                        It's an integral part of Goan culture and is often enjoyed during festivals.Goa's history, culture,
                        and cuisine create a unique blend that makes it a captivating destination, offering travelers a
                        chance to explore its diverse heritage and indulge in its flavorful culinary delights.

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
            <a href="/app" class="a">Customize your own Package</a>
        </div>
        <footer>
            <div id="footer-top" class="social-footer">
                <div class="container">
                    <div class="region region-footer-top">
                        <div id="block-block-1" class="block block-block">
                            <div class="content">
                                <div class="col-md-12 sf-icons">
                                    <a href="#" target="_blank"><i class="fa fa-twitter" style="color: #ffffff;"> </i></a>
                                    &nbsp;
                                    &nbsp;&nbsp;&nbsp;
                                    <a href="#" target="_blank"><i class="fa fa-facebook"
                                            style="color: #ffffff;"></i></a>&nbsp;&nbsp;&nbsp;&nbsp;
                                    <a href="#" target="_blank"><i class="fa fa-instagram"
                                            style="color: #ffffff;"></i></a>&nbsp;&nbsp;&nbsp;&nbsp;
                                    <a href="#" target="_blank"><i class="fa fa-youtube"
                                            style="color: #ffffff;"></i></a>&nbsp;&nbsp;&nbsp;&nbsp;
                                    <a href="#" target="_blank"><i class="fa fa-telegram"
                                            style="color: white;"></i></a>&nbsp;&nbsp;&nbsp;&nbsp;
                                </div>
                                <br>
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

@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,300;0,400;0,600;1,200;1,300;1,400;1,700&family=Roboto:ital,wght@1,300&display=swap');

* {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    /* background-color: #c1f5d0; */
}

.body {
    font-family: 'Poppins', sans-serif;
    /* z-index: -100; */
    /* background-color: #c1f5d0; */
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
    color: #070F57;
}

header nav h3 span {
    color: #FD7200;
}

header nav ul {
    list-style: none;
    display: flex;

}

header nav ul li {
    padding: 3px 15px;

}

header nav ul li:nth-last-child(1) {
    background: #070F57;
    border-radius: 20px;
    padding: 5px 20px;
}

header nav ul li:nth-last-child(1):hover {
    background: #070F57;
}

header nav ul li:nth-last-child(1) a:hover {
    color: black;
}

header nav ul li:nth-last-child(1) a {
    color: white;
}

header nav ul li a {
    text-decoration: none;
    color: #070F57;
    font-size: 17px;
    font-weight: bold;
    transition: .3s linear;
}


header nav ul li a:hover {
    color: #FD7200;

}

header nav .bi-three-dots {
    display: none;
}

header .content {
    position: relative;
    height: 80%;
    width: 100%;
    /* border: 2px solid red; */
}

header .content::before {
    content: '';
    position: absolute;
    width: 100%;
    height: 80%;
    background: url("~/staticc/goa1.jpg")no-repeat center center/cover;
    border-radius: 10px;
    z-index: -1;
    /* border: 2px solid red; */
}

header .content .cont {
    width: 700px;
    height: auto;
    color: #d8fcd8;
    padding: 30px;
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
    border: 2px solid #FD7200;
    background: #FD7200;
    color: white;
    outline: none;
    cursor: pointer;
    transition: .3s linear;
    text-decoration: none;
    font-size: 17px;
    font-weight: bold;

}

header .content .cont a:hover {
    background: #070F57;
    border: 1px solid #070F57;
}


.cardholder {
    display: flex;
}

.card {
    display: block;
    width: 22%;
    /* background-color: rgb(7, 126, 21); */
    background-color: #FD7200;
    border-radius: 25%;
    padding: 30px 20px;
    margin: 0px 20px;
    box-shadow: 0px 0px 10px #FD7200;
    border: 2px solid white;
    color: white;
    opacity: 0.9;
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
}

.whole {
    margin-left: 5%;
    margin-top: 5%;
    width: 90%;
    border: 2px solid blue;
    border-radius: 12%;
    box-shadow: 0px 0px 20px 070F57;
    background-color: #070F57;
}

.trip {
    position: relative;
    width: 95%;
    height: auto;
    margin-left: 7%;
    margin-top: 5%;
    /* text-align: center; */
    color: #FD7200;
    /* border: 1px solid green; */
}

.trip h3 {
    font-size: 20px;
    text-shadow: 0px 0px 10px FD7200;
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
    text-shadow: 0px 0px 10px #FD7200;
    font-size: 1.2rem;
    /* border: 1px solid red; */
    /* margin-left: 10%; */
}

.trip .info img {
    position: absolute;
    right: 5%;
    width: 40%;
    border: 2px solid #FD7200;
    border-radius: 20px;
    box-shadow: 0px 0px 20px #FD7200;
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
    border: 2px solid #070F57;
    background: #070F57;
    color: #FD7200;
    outline: none;
    cursor: pointer;
    text-align: center;
    text-decoration: none;
    font-size: 13px;
    font-weight: bold;
    /* transition: .3s linear; */

}

.button .a:hover {
    background: #070F57;
    border: 1px solid #070F57;
}

footer {
    background-color: #070F57;
    color: #FD7200;
    margin-top: 6.35%;
    padding: 20px;
    text-align: center;
    width: 100%
        /* opacity: 0.6; */
        /* z-index: ; */
        /* border: 2px solid green; */

}
</style>
  
  <!-- <script>
  export default {
    name: 'KeralaInfo',
    // Any JavaScript functionality goes here
  }
  </script> -->
  
  