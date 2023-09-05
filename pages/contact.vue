<template>
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
    <div class="contact-page">
        <section class="contact-form">
            <h1>Contact Us</h1><br>
            <p>Have questions or want to book a tour? Get in touch with us!</p><br>
            <form @submit="submitForm">
                <div class="form-group">
                    <label for="name">Your Name</label><br>
                    <input type="text" id="name" v-model="formData.name" required />
                </div><br>
                <div class="form-group">
                    <label for="email">Email Address</label><br>
                    <input type="email" id="email" v-model="formData.email" required />
                </div><br>
                <div class="form-group">
                    <label for="message">Message</label><br>
                    <textarea id="message" v-model="formData.message" rows="5" required></textarea>
                </div><br>
                <button type="submit">Submit</button>
            </form>
        </section>
        <br>
        <section class="contact-details">
            <h2>Contact Details</h2><br>
            <p>If you prefer other methods of communication, feel free to reach out to us:</p><br>
            <p>Phone: <a class="contact" href="#">9993332221</a></p><br>
            <p>Email: <a class="contact" href="#">Travelopedia65@gmail.com</a></p><br>
            <p>Address: <a class="contact" href="#">Ramnarain Ruia College</a></p><br>

        </section>
    </div>
</template>
  
<script>
export default {
    data() {
        return {
            formData: {
                name: '',
                email: '',
                message: ''
            }
        };
    },
    methods: {
        submitForm() {
            // You can implement form submission logic here, like sending the form data to a backend server.
            console.log('Form submitted:', this.formData);
            // Reset the form fields
            this.formData = {
                name: '',
                email: '',
                message: ''
            };
        }
    }
};
</script>
  
<style scoped>
* {
    margin: 0;
    padding: 0;
    /* box-sizing: border-box; */
    /* border: 2px solid red; */


}



.contact-page {
    width: 100%;
    display: block;
    /* justify-content: space-between; */
    margin: 50px auto;
    max-width: 1200px;
    padding: 20px;
    justify-content: center;
    color: white;
}

.contact-form {
    flex: 1;
    /* position: absolute; */
    /* left: 40%; */
    /* border: 2px solid black; */
}

.contact-details {
    /* flex: 2; */
    /* background-color: #3e8adb; */
    margin-bottom: 0%;
    display: block;
    color: white;
    text-decoration: none;
}

.contact-details a {
    /* flex: 2; */
    /* background-color: #3e8adb; */

    color: white;
    text-decoration: none;
}



label {
    display: block;
    font-weight: bold;
}

input,
textarea {
    width: 50%;
    padding: 10px;
    border: 3px solid orange;
    border-radius: 4px;
    background: rgb(224, 216, 216);
}

button {
    padding: 10px 20px;
    background-color: orange;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
}

button:hover {
    background-color: rgb(215, 140, 0);
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
    /* text-decoration: none; */
    color: white;
    text-decoration: none;

    /* transition: all .5s; */
}

.navbar a p {
    text-decoration: none;
    color: white;

    /* transition: all .5s; */
}

.navbar a:hover {
    text-decoration: underline;
    /* color: white; */
}
</style>
  