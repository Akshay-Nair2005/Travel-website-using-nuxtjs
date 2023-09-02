<template>
    <div class="body">
        <div class="cover">
            <h1 class="pack">Package Offer!!!!</h1>
            <div class="container">
                <div class="img">
                    <h1>Custom Package</h1>
                    <p class="Desc">Enjoy your trip to fullest......</p>
                    <p class="Rate"><strong>Rate: Rs ###</strong></p>
                </div>
                <div class="custom">
                    <div class="serv">
                        <img class="hotel1" src="./static/hotel1.jpg" alt="hotel">
                        <h3>Hotel</h3>
                        <p>
                            <!-- Your hotel description here -->
                            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dolore nemo aut et molestias omnis
                            optio, sapiente quo sequi eveniet unde dolorem totam eligendi rem eos. Lorem, ipsum dolor sit
                            amet consectetur adipisicing elit. Lorem ipsum dolor sit amet.
                        </p>
                    </div>
                    <div class="serv">
                        <img class="plane" src="./static/plane1.jpg" alt="plane">
                        <h3>Flight</h3>
                        <p>
                            <!-- Your flight description here -->
                            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quidem voluptatum obcaecati soluta eos
                            nihil, quaerat minus veritatis animi accusantium reprehenderit neque natus rerum quibusdam
                            maxime. Lorem ipsum dolor sit amet consectetur adipisicing elit. Ab voluptatibus,Lorem ipsum
                            dolor sit amet.
                        </p>
                    </div>
                    <div class="serv">
                        <img class="person" src="./static/c_c4.jpg" alt="shinchan">
                        <h3>Travel Guide</h3>
                        <p>
                            <!-- Your travel guide description here -->
                            Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto, autem sunt nesciunt recusandae
                            odit quasi voluptatibus molestiae ipsam neque modi, minima, obcaecati excepturi nam non!
                        </p>
                    </div>
                </div>
            </div>
            <br>
            <!-- <a href="#">Book Now</a> -->
            <nuxt-link to="/pay" class="a">Explore</nuxt-link>
            <!-- <script src="~/assets/font.js"></script> -->
        </div>
    </div>
</template>
  
<style scoped>
/* Your CSS styles here */
.body {
    margin: 0px;
    padding: 0px;
    background: url('~/staticc/kerala_bg.jpg') no-repeat center center/cover;
    color: white;
    z-index: 100;
    height: 100%;
    /* opacity: 0.7; */
    /* background-color: teal; */
    /* background : url('../kerala_sport.gif') no-repeat center center/cover; */

}

.head {
    text-align: center;
}

.cover {
    width: 91%;
    opacity: 0.9;
    height: 80%;
    text-align: center;
    margin-left: 5%;
    margin-bottom: 5%;
    padding: 20px 20px;
    background-color: transparent;
    color: azure;
    border-radius: 7px;
    z-index: 200;
    /* border: 2px solid black; */
    /* background : url('../kerala/kerala_bg1.jpg') no-repeat center center/cover; */
    /* box-shadow: 0px 0px 45px black; */
    /* border: 2px solid red; */
    /* margin-right: 40%; */
}

.container {
    z-index: 500;
    display: flex;
    height: 50%;
    /* border: 2px solid red; */
    /* justify-content: center; */
    /* width: 80%;
            /* align-items: center; */
}

.kerala {
    height: 70%;
}

.img {
    font-size: 2rem;
    color: azure;
    /* width: 200%; */
    /* border: 2px solid red; */
}

.Desc {
    font-size: 36px;
    /* font-weight: bold; */
    text-align: left;
    color: azure;
}

.custom img {
    width: 100%;
    height: 20%;
    border: 2px solid black;
    border-radius: 5px;

}

.person {
    height: 5%;
}


p {
    padding-top: 20px;
    margin-bottom: 0px;
    /* opacity: 1; */
    /* color: black; */

}

.Rate {
    font-size: 25px;
    color: azure;
}

.pack {
    margin-left: 35%;
    font-size: 38px;
    color: azure;
    transition: all 0.5s ease .1s;
    /* transition-property: background-color box-shadow;
            transition-duration: 2s;
            transition-timing-function: ease-in-out;
            transition-delay: 2s; */
    /* color: white; */
}


/* @keyframes 
        .pack:hover {
            font-size: 45px;
            
        } */

.custom {
    display: flex;
    margin: 0px 100px;
    height: 60%;
    z-index: 1000;
    /* background-color: black; */
    /* box-shadow: 0px 0px 45px black; */
    /* width: 20%; */
    /* border: 2px solid red; */

}

.serv {
    width: 33%;
    box-shadow: 0px 0px 45px black;
    border-radius: 5px;
    margin: 2px 25px;
    padding: 10px 14px;
    text-align: center;
    background-color: black;
    color: azure;
    border: 2px solid azure;
    height: 80%;
    /* background-color: transparent; */
    /* background-color: rgb(127, 151, 139); */
    /* background : url('../kerala/kerala_bg1.jpg') no-repeat center center/cover; */
    /* opacity: 0.6; */
    /* height: 500px; */
    /* background : url('../beach1.jpg') no-repeat center center/cover; */
}


.serv:hover {
    font-size: 15px;
    font-weight: bold;
    /* color: black; */
    /* background-color: azure; */
    /* height: 20%; */
    /* width: 120%; */
    /* transition: width 0.5s ease-in-out; */
    transform: scale(1.1);
}



.services {
    /* width: 33%; */
    font-weight: bolder;
    color: azure;
    font-size: 22px;
    text-align: center;
}

/* .hotel1 {
            height: 50%;
        } */

/* h1 { */
/* width: 50%; */
/* font-size: 20px; */
/* } */

.a {
    display: inline-block;
    background-color: black;
    box-shadow: 0px 3px 45px black;
    color: rgb(218, 243, 243);
    font-size: 25px;
    font-weight: bold;
    padding: 10px 20px;
    text-decoration: none;
    border-radius: 5px;
    margin-top: 2%;
    border: 2px solid azure;
    margin-left: 19%;
    width: 58%;
    text-align: center;
    /* margin-bottom: 5%; */
}

/* Mobile-first responsive design */
@media screen and (max-width: 768px) {
    .cover {
        width: 95%;
        margin-left: 2.5%;
        padding: 10px;
    }

    .container {
        flex-direction: column;
        align-items: center;
    }

    .img {
        font-size: 1.5rem;
        text-align: center;
        margin: 10px 0;
    }

    .custom {
        flex-direction: column;
        align-items: center;
        margin: 10px 0;
    }

    .serv {
        width: 80%;
        margin: 10px 0;
    }

    a {
        width: 80%;
        margin: 10px 10%;
    }
}
</style>
  
<!-- <script>
window.addEventListener('load', function () {
    const pack = document.querySelector('.pack');
    const initialFontSize = parseInt(getComputedStyle(pack).fontSize); // Get the initial font size in pixels
    const targetFontSize = 36; // Set the target font size in pixels (increase)
    const intervalTime = 1000; // Set the interval time in milliseconds

    // Increase font size after a short delay
    setTimeout(function () {
        pack.style.fontSize = targetFontSize + 'px';
    }, intervalTime);

    // Decrease font size back to the initial size after another short delay
    setTimeout(function () {
        pack.style.fontSize = initialFontSize + 'px';
    }, intervalTime * 2);
});
</script> -->
  