<template>
    <div class="cont">
        <div class="container1">
            <div class="payment-form">
                <h1>Payment Gateway</h1>
                <form action="#" method="post">
                    <div class="contents">
                        <div class="form-group">
                            <input type="text" id="cardNumber" placeholder="Enter your card number (16 digits)" required
                                v-model="cardNumber" @input="validateCardNumber" maxlength="16" /><br><br>
                            <span class="error" v-if="!isCardNumberValid">Invalid card number</span>
                        </div>
                        <div class="form-group">
                            <input type="text" id="name" placeholder="Enter cardholder's name" required />
                        </div>
                        <div class="form-row">
                            <div class="form-group">
                                <input type="text" id="expiry" placeholder="MM / YY" required maxlength="4" />
                            </div>
                            <div class="form-group">
                                <input type="password" id="cvv" placeholder="CVV (3 digits)" required v-model="cvv"
                                    @input="validateCVV" maxlength="3" /><br><br>
                                <span class="error" v-if="!isCVVValid">Invalid CVV</span>
                            </div>
                        </div>
                        <button type="button" class="pay-btn" @click="handlePayment"
                            :disabled="!isCardNumberValid || !isCVVValid">
                            Pay Now
                        </button>
                        <!-- <a href="/hotels">click me</a> -->
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
    background: url('~/staticc/nature3.jpg') no-repeat center center/cover;
    /* background-color: black; */
    opacity: 5;
}

.container1 {
    width: 50%;
    padding: 40px 40px;
    /* background: url('../pay_bg1.jpg') no-repeat center center/cover; */
    /* background: url('../nature4.jpg') no-repeat center center/cover; */
    border: 2px solid white;
    box-shadow: 0 2px 45px azure;
    border-radius: 8px;
    color: white;
    background-color: black;
    opacity: 0.85;
    z-index: 1000;
}


h1 {
    text-align: center;
    margin-bottom: 20px;
    color: white;
}

label {
    font-weight: bold;
}

input {
    width: 90%;
    padding: 10px;
    border: 1px solid white;
    border-radius: 4px;
    background: none;
    color: white;
    /* color: black; */
}

input::placeholder {
    color: white;
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
    /* display: black; */
    width: 60%;
    padding: 10px;
    margin-top: 25px;
    margin-left: 12%;
    background-color: transparent;
    border: 2px solid white;
    color: white;
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
    data() {
        return {
            cardNumber: "",
            cvv: "",
            isCardNumberValid: false,
            isCVVValid: false,
        };
    },
    methods: {
        handlePayment() {
            // Simulate successful payment for demonstration purposes
            // In a real implementation, you would handle the payment processing logic here
            // and then trigger the alert upon successful payment.
            // For demonstration, we'll just show an alert immediately.
            alert("Payment Successful! Thank you for your payment.");
        },
        validateCardNumber() {
            // Check if the card number is exactly 16 digits
            this.isCardNumberValid = /^\d{16}$/.test(this.cardNumber);
        },
        validateCVV() {
            // Check if the CVV is exactly 3 digits
            this.isCVVValid = /^\d{3}$/.test(this.cvv);
        },
    },
};
</script>