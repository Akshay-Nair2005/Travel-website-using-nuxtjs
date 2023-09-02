<template>
    <div class="body">
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
        <div class="container">
            <h1>Tourism Booking Form</h1>
            <form id="booking-form" name="booking-form" @submit="submitForm">
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" v-model="formData.name" required>

                <label for="email">Email:</label>
                <input type="email" id="email" name="email" v-model="formData.email" required>

                <label for="destination">Destination:</label>
                <select id="dest-loc" name="dest" v-model="formData.dest" required>
                    <option value="Dubai">Dubai</option>
                    <option value="Singapore">Singapore</option>
                    <option value="London">London</option>
                    <option value="Kerala">Kerala</option>
                    <option value="Goa">Goa</option>
                    <option value="Himachal_Pradesh">Himachal Pradesh</option>
                </select>

                <label for="flight-type">Flight Type:</label>
                <select id="flight-type" name="flight-type" v-model="formData.flightType">
                    <option value="business">Business</option>
                    <option value="economy">Economy</option>
                </select>

                <label for="train-type">Train Type:</label>
                <select id="train-type" name="train-type" v-model="formData.trainType">
                    <option value="2-tier">2 Tier</option>
                    <option value="3-tier">3 Tier</option>
                </select>

                <label for="no-of-people">Number of Passengers:</label>
                <input type="number" id="Passengers" name="Passengers" v-model="formData.passengers" required>

                <label for="hotel-charges">Hotel Charges:</label>
                <input type="number" id="hotel-charges" name="hotel-charges" v-model="formData.hotelCharges">

                <label for="guide-charges">Travel Guide Charges:</label>
                <input type="number" id="guide-charges" name="guide-charges" v-model="formData.guideCharges">

                <button type="submit">Submit</button>
            </form>
        </div>
    </div>
</template>
  
<script>
export default {
    data() {
        return {
            formData: {
                name: '',
                email: '',
                dest: '',
                flightType: 'business',
                trainType: '2-tier',
                passengers: '',
                hotelCharges: '',
                guideCharges: '',

            },
        };
    },
    methods: {
        async submitForm(event) {
            event.preventDefault();


            try {
                const response = await this.$axios.post(
                    'https://script.google.com/macros/s/AKfycbynYGcKrGKx_qbVPlkUkXdiDD7yMOUgi3-vIEcegYlJ46mBbvujHct1hrwblduGYpwW2A/exec',
                    this.formData,
                    console.log(response)
                );

                if (response.status === 200) {
                    alert('Form submitted successfully!');
                    this.$refs.form.reset();
                } else {
                    alert('Form submission failed.');
                }
            } catch (error) {
                alert('An error occurred while submitting the form.');
            }
        },
    },
};
</script>
  
<style scoped>
/* Your existing styles... */
.body {
    margin: 0;
    font-family: Arial, sans-serif;
    margin: 0px;
    padding: 0px;
    /* background: url('../page1/beach1.jpg') no-repeat center center/cover; */
    /* background-color: rgb(22, 59, 128); */
}

header {
    background-color: rgb(3, 34, 90);
    /* position: sticky; */
    top: 0;
    /* background: url('../page2/beach1.jpg') no-repeat center center/cover; */
    /* opacity: 0.5; */
}

.navbar {
    justify-content: center;
    padding: 10px 0;
    /* z-index: 1; */
    /* text-align: center; */
    /* border: 2px solid red; */
}

ul {
    display: flex;
    z-index: 1000;
    list-style: none;
    margin-left: 31%;
    /* border: 2px solid red; */
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

label {
    display: block;
    margin-top: 10px;
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
  
