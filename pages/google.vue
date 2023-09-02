<template>
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
    <div class="head">
        <p>
            Customize your Own Package!!!!
        </p>
    </div>
    <div class="whole">
        <div class="iframe-container">
            <iframe
                src="https://docs.google.com/forms/d/e/1FAIpQLSeGn5SgXeKkpycivIDiaoDpnOfX5maTMmyZbL3nQxOi60I9Xw/viewform?embedded=true"
                width="640" height="1257" frameborder="0" marginheight="0" marginwidth="0">Loading…
            </iframe>
        </div>
        <div class="info">


            <div class="container1">
                <div class="payment-form">
                    <h1>Payment Gateway</h1>
                    <form action="#" method="post">
                        <div class="contents">
                            <div class="form-group">
                                <input type="text" id="cardNumber" placeholder="Enter your card number" required />
                            </div>
                            <div class="form-group">
                                <input type="text" id="name" placeholder="Enter cardholder's name" required />
                            </div>
                            <div class="form-row">
                                <div class="form-group">
                                    <input type="text" id="expiry" placeholder="MM / YY" required />
                                </div>
                                <div class="form-group">
                                    <input type="password" id="cvv" placeholder="CVV" required />
                                </div>
                            </div>
                            <button type="submit" class="pay-btn">Pay Now</button><br><br><br>
                        </div>
                    </form>
                </div>
            </div>
        </div>
    </div>
</template>
  

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
    border-radius: 5px;
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
    overflow: hidden;
    padding-top: 3%;
    width: 50%;
    /* 16:9 aspect ratio */
}

.embedded-iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 120%;
    height: 100%;
}

.whole {
    display: flex;
    border: 5px solid rgba(3, 34, 90, 0.9);
    border-radius: 0px;
    border-top: none;
    border-bottom: none;
}

.info {
    display: block;
}

.cont {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background-color: #f0f0f0;
    /* background: url('../pay_bg1.jpg') no-repeat center center/cover; */
}

.container1 {
    width: 45%;
    margin-top: 25%;
    /* padding: 40px 40px; */
    /* background: url('../pay_bg1.jpg') no-repeat center center/cover; */
    border: 2px solid black;
    box-shadow: 0 2px 45px white;
    border-radius: 8px;
    background-color: white;
    height: 150%;
}


h1 {
    text-align: center;
    margin-bottom: 20px;
    color: black;
}

label {
    font-weight: bold;
}

input {
    width: 90%;
    padding: 10px;
    border: 1px solid black;
    border-radius: 4px;
    background: none;
    color: black;
}

input::placeholder {
    color: black;
}

.form-row {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 80%;
    /* margin: 0px 5px; */
}

.form-group {
    width: 80%;
    /* margin: 0px 15px; */
    margin-left: 20px;
    padding: 10px 15px;
}

.pay-btn {
    display: black;
    width: 60%;
    padding: 10px;
    margin-top: 25px;
    margin-left: 12%;
    background-color: transparent;
    border: 2px solid black;
    color: black;
    /* border: none; */
    border-radius: 4px;
    cursor: pointer;
    font-size: 16px;
    font-weight: bold;
    /* transition: background-color 0.3s ease; */
}


.contents {
    /* display: flex; */
    width: 80%;
    margin-left: 15%;
    padding-left: 1%;
}
</style>
  