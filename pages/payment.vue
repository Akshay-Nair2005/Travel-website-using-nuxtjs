<template>
    <div class="cont">
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
                        <button type="button" class="pay-btn" @click="handlePayment">Pay Now</button>
                    </div>
                </form>
            </div>
        </div>
    </div>
</template>
  
<style scoped>
/* Your CSS styles here */
.cont {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background-color: white;
    /* background: url('../pay_bg1.jpg') no-repeat center center/cover; */
}

.container1 {
    width: 50%;
    padding: 40px 40px;
    /* background: url('../pay_bg1.jpg') no-repeat center center/cover; */
    border: 2px solid black;
    box-shadow: 0 2px 45px azure;
    border-radius: 8px;
    background-color: white;
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
  
<script>
export default {
    methods: {
        handlePayment() {
            // Simulate successful payment for demonstration purposes
            // In a real implementation, you would handle the payment processing logic here
            // and then trigger the alert upon successful payment.
            // For demonstration, we'll just show an alert immediately.
            alert('Payment Successful! Thank you for your payment.');
        },
    },
};
</script>
  