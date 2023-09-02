<template>
    <div>
        <header>
            <nav class="navbar">
                <ul>
                    <li><nuxt-link to="/">Home</nuxt-link></li>
                    <li><nuxt-link to="/about">About</nuxt-link></li>
                    <li><nuxt-link to="/services">Services</nuxt-link></li>
                    <li><nuxt-link to="/contact">Contact</nuxt-link></li>
                </ul>
            </nav>
        </header>
        <div class="container">
            <h1>Tourism Booking Form</h1>
            <!-- <form id="booking-form" name="booking-form"> -->
            <!-- Your form content -->
            <form ref="bookingForm" @submit.prevent="submitForm">
                <!-- Form fields here -->
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" required>
                <br><br>
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required>
                <br><br>
                <label for="destination">Destination:</label>
                <select id="dest-loc" name="dest" required>
                    <option value="Dubai">Dubai</option>
                    <option value="Singapore">Singapore</option>
                    <option value="London">London</option>
                    <option value="Kerala">Kerala</option>
                    <option value="Goa">Goa</option>
                    <option value="Himachal_Pradesh">Himachal Pradesh</option>
                </select>
                <br><br>
                <label for="flight-type">Flight Type:</label>
                <select id="flight-type" name="flight-type">
                    <option value="business">Business</option>
                    <option value="economy">Economy</option>
                </select>
                <br><br>
                <label for="train-type">Train Type:</label>
                <select id="train-type" name="train-type">
                    <option value="2-tier">2 Tier</option>
                    <option value="3-tier">3 Tier</option>
                </select>
                <br><br>
                <label for="no-of-people">Number of Passengers:</label>
                <input type="number" id="Passengers" name="Passengers" required>
                <br><br>
                <label for="hotel-charges">Hotel Charges:</label>
                <input type="number" id="hotel-charges" name="hotel-charges">
                <br><br>
                <label for="guide-charges">Travel Guide Charges:</label>
                <input type="number" id="guide-charges" name="guide-charges">
                <br><br>
                <button type="submit">Submit</button>
            </form>
        </div>
    </div>
</template>

<script>
export default {


    methods: {

        async submitForm() {
            // Get form data from the ref
            const formData = new FormData(this.$refs.bookingForm);
            console.log(formData)

            // Convert form data to a plain object
            const formDataObject = {};
            formData.forEach((value, key) => {
                formDataObject[key] = value;
            });

            // Save form data to JSON file
            try {
                await this.$axios.post('/api/saveFormData', formDataObject);
                alert('Form data submitted and saved.');
            } catch (error) {
                console.log('Error submitting form:', error);
            }
        }
    }
};


</script>

<style scoped>
body {
    margin: 0;
    font-family: Arial, sans-serif;
    margin: 0px;
    padding: 0px;
}

header {
    background-color: rgb(3, 34, 90);
}

.navbar {
    justify-content: center;
    padding: 10px 0;
}

ul {
    display: flex;
    z-index: 1000;
    list-style: none;
    margin-left: 31%;
}

li {
    margin: 0 15px;
}

a {
    color: #fff;
    text-decoration: none;
    padding: 5px 10px;
}

a:hover {
    background-color: rgb(3, 3, 71);
    border-radius: 5px;
    color: white;
}

.container {
    max-width: 60%;
    margin: 25px auto;
    padding: 20px;
    border: 1px solid #ccc;
    border-radius: 5px;
}

.container h1 {
    text-align: center;
}

input,
select {
    width: 80%;
    padding: 8px;
    margin-top: 2%;
    border: 1px solid #ccc;
    border-radius: 3px;
    margin-left: 10%;
}

label {
    margin-left: 10%;
}

input {
    width: 78%;
    padding: 8px;
    margin-top: 4px;
    border: 1px solid #ccc;
    border-radius: 3px;
    margin-left: 10%;
}

button {
    display: block;
    margin-left: 8%;
    width: 85%;
    margin-top: 5%;
    padding: 10px;
    background-color: rgb(3, 3, 71);
    color: white;
    border: none;
    border-radius: 3px;
    cursor: pointer;
}

button:hover {
    background-color: #007BFF;
}
</style>


  
<!-- export default {
    data() {
        return {
            name: '',
            email: '',
            destination: '',
            flightType: '',
            trainType: '',
            passengers: 0,
            hotelCharges: 0,
            guideCharges: 0
        };
    },
    methods: {
        async submitForm() {
            const formData = {
                name: this.name,
                email: this.email,
                destination: this.destination,
                flightType: this.flightType,
                trainType: this.trainType,
                passengers: this.passengers,
                hotelCharges: this.hotelCharges,
                guideCharges: this.guideCharges
            };

            try {
                const response = await this.$axios.post('/api/submit', formData);
                console.log(response.data.message);
                alert("The Data is Submitted");
            } catch (error) {
                console.error('Error submitting form:', error);
            }
        }
    }
}; -->

<!-- Error submitting form: TypeError: Cannot read properties of undefined (reading 'post')
    at Proxy.submitForm (Customize1.vue:81:35)
    at Customize1.vue:17:54
    at chunk-BVQHDTV7.js:10436:12
    at callWithErrorHandling (chunk-BVQHDTV7.js:1565:18)
    at callWithAsyncErrorHandling (chunk-BVQHDTV7.js:1573:17)
    at HTMLFormElement.invoker (chunk-BVQHDTV7.js:9397:5) -->