<template>
    <header>
        <nav class="navbar">
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#contact">Contact</a></li>
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
}



label {
    display: block;
    font-weight: bold;
}

input,
textarea {
    width: 50%;
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 4px;
}

button {
    padding: 10px 20px;
    background-color: #007bff;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
}

button:hover {
    background-color: #0056b3;
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

.contact {
    color: black;

}

.contact:hover {
    background-color: white;
    color: black;

}
</style>
  