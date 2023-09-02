
<template>
    <div class="body">
        <nav id="navbar">
            <div id="logo">
                <img src="./static/logoo.png" alt="logo" />
                <h1 class="Akki">Travelopedia</h1>
            </div>

            <ul class="unordy">
                <!-- <li class="item"><a href="index.vue">Destination</a></li>
                <li class="item"><a href="#">About us</a></li>
                <li class="item"><a href="#">Help</a></li>
                <li class="item"><a href="#">Contact</a></li> -->
                <li class="item"><nuxt-link to="/destination">Destination</nuxt-link></li>
                <li class="item"><nuxt-link to="/about">About Us</nuxt-link></li>
                <li class="item"><nuxt-link to="/review">Review</nuxt-link></li>
                <li class="item"><nuxt-link to="/contact">Contact</nuxt-link></li>
                <li class="item"><nuxt-link to="/present">Presentation</nuxt-link></li>
            </ul>
        </nav>

        <section id="home">
            <h1 class="head">Welcome to Kingdom of Heaven</h1>
            <p>Explore your dreams with us.... within and beyond the borders </p>
            <p>"Where Dreams come alive..."</p>
            <p>- Akshay Nair</p>
            <!-- <a href="index.vue" class="a" target="_blank">Explore</a> -->
            <nuxt-link to="/destination" class="a">Explore</nuxt-link>
        </section>

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
/* CSS reset and other styles... */
/* css reset */

* {
    margin: 0;
    padding: 0;
    /* background-color: black; */
}

.body {
    /* border: 2px solid red; */
    padding: 0;
}

:root {
    --navbar-height: 59px;


}


/* Navigation Bar */
#navbar {
    display: flex;
    align-items: center;
    /* justify-content: center; */
}

/* Nav: Logo and image */

#logo {
    margin: 34px 25px;

}

#logo img {

    margin: -22px 5px;
    height: 110px;
    width: 150px;

}

/* ChefYChef */
.Akki {
    font-size: 2.0rem;
    color: white;
    display: flex;
    position: absolute;
    font-family: 'Poppins', cursive;
    /* padding-left: 10px; */
    text-align: left;
    /* align-items: left; */
    /* justify-content: flex-start; */
    margin: 5px 5px;

}

/* .Akki h1::before {
        z-index: -1;
    } */

/* Nav: Listing Items */

#navbar {
    position: relative;
    /* width: 100%; */
}

#navbar::before {
    content: "";
    background-color: black;
    position: absolute;
    height: 120%;
    width: 100%;
    z-index: -1;
    opacity: 1;
}

#navbar ul {
    display: flex;

}


#navbar ul li {
    /* color: white;     */
    list-style: none;
    font-size: 1.2rem;
}

#navbar ul li a {
    display: block;
    padding: 5px 40px;
    border-radius: 7px;
    text-decoration: none;
    color: azure;
    font-family: 'Bree Serif', serif;
    font-size: 1.5rem;
}

#navbar ul li a:hover {
    color: azure;
    font-size: 1.7rem;
    /* background-color: white; */
    /* text-decoration: underline; */
}

/* home section */

#home {
    display: flex;
    flex-direction: column;
    padding: 3px 200px;
    margin-top: 4%;
    justify-content: center;
    align-items: center;
    /* position: relative; */
    height: 290px;

}

#home::before {
    content: "";
    background: url('~/staticc/Bgimage_home.webp') no-repeat center center/cover;
    position: absolute;
    /* border: 2px solid red; */
    /* height: 80%; */
    height: 110%;
    width: 100%;
    z-index: -1;
    opacity: 0.89;
}

#home h1 {
    color: white;
    text-align: center;
    font-family: 'Bree Serif', serif;
    text-shadow: 3px 5px 3px rgb(209, 207, 207);

}

#home h1:hover {
    transform: scale(1.05);
}

#home p {
    color: azure;
    text-align: center;
    font-size: 1.5rem;
    font-family: 'Bree Serif', serif;
}







/* utility class */

.head {
    font-size: 4.0rem;
    padding: 12px;
    margin-top: 10%;

}

.secondary {
    font-size: 2.8rem;
    padding: 12px;

}


.a {
    padding: 6px 25px;
    color: white;
    border: 2px solid white;
    background-color: transparent;
    margin: 7%;
    font-size: 1.5rem;
    border-radius: 10px;
    font-family: 'Bree Serif', serif;
    cursor: pointer;
    text-decoration: none;
}

.a:hover {
    transform: scale(1.2);
}

/* Footer */
footer {
    background-color: #aa1e48;
    color: #fff;
    margin-top: 10%;
    padding: 20px;
    text-align: center;
    opacity: 0.6;
    /* z-index: ; */
    /* border: 2px solid green; */

}

.foot {
    z-index: -1;
    color: white;
}

/* .row {
        width: 100%;
        background-color: #aa1e48;
    } */

/* Mobile-first responsive design */
@media screen and (max-width: 768px) {
    #logo {
        margin: 10px;
    }

    .Akki {
        font-size: 1.5rem;
        margin: 5px;
    }

    #navbar {
        flex-direction: column;
        align-items: flex-start;
        position: relative;
    }

    #navbar::before {
        opacity: 0.6;
    }

    #navbar ul {
        flex-direction: column;
        align-items: center;
        background-color: rgba(0, 0, 0, 0.8);
        position: absolute;
        top: var(--navbar-height);
        width: 100%;
        left: 0;
        display: none;
    }

    #navbar.active ul {
        display: flex;
    }

    #navbar ul li {
        padding: 10px;
        width: 100%;
        text-align: center;
    }

    #home {
        padding: 10px;
        height: auto;
    }

    #home::before {
        opacity: 0.5;
    }

    #home h1 {
        font-size: 2.5rem;
    }

    #home p {
        font-size: 1rem;
    }

    .head {
        font-size: 2rem;
        padding: 8px;
    }

    .a {
        font-size: 1rem;
        margin: 10px;
        padding: 5px 15px;
    }

    footer {
        margin-top: 20%;
        padding: 10px;
    }
}
</style>
    