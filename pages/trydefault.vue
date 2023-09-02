<template>
    <div class="custom-package">
        <section class="package-header">
            <h1>Custom Travel Package to Kerala</h1>
            <p>Experience the beauty of Kerala with our personalized package</p>
        </section>
        <section class="package-options">
            <h2>Choose Your Options</h2>
            <div class="option">
                <h3>Hotels</h3>
                <select v-model="selectedHotel">
                    <option v-for="hotel in hotels" :key="hotel.id">{{ hotel.name }}</option>
                </select>
            </div>
            <div class="option">
                <h3>Flights</h3>
                <select v-model="selectedFlight">
                    <option v-for="flight in flights" :key="flight.id">{{ flight.name }}</option>
                </select>
            </div>
            <div class="option">
                <h3>Travel Guides</h3>
                <select v-model="selectedGuide">
                    <option v-for="guide in guides" :key="guide.id">{{ guide.name }}</option>
                </select>
            </div>
            <div class="option">
                <h3>Travel Planning</h3>
                <textarea v-model="travelPlan" rows="5" placeholder="Tell us more about your travel preferences"></textarea>
            </div>
        </section>
        <section class="package-summary">
            <h2>Your Package Summary</h2>
            <p><strong>Hotel:</strong> {{ selectedHotel }}</p>
            <p><strong>Flight:</strong> {{ selectedFlight }}</p>
            <p><strong>Travel Guide:</strong> {{ selectedGuide }}</p>
            <p><strong>Travel Plan:</strong> {{ travelPlan }}</p>
            <button @click="submitPackage">Submit Package</button>
        </section>
    </div>
</template>
  
<script>
export default {
    data() {
        return {
            selectedHotel: '',
            selectedFlight: '',
            selectedGuide: '',
            travelPlan: '',
            hotels: [
                { id: 1, name: 'Luxury Resort' },
                { id: 2, name: 'Cozy Cottage' },
                // Add more hotel options
            ],
            flights: [
                { id: 1, name: 'Flight A' },
                { id: 2, name: 'Flight B' },
                // Add more flight options
            ],
            guides: [
                { id: 1, name: 'Local Expert 1' },
                { id: 2, name: 'Local Expert 2' },
                // Add more guide options
            ],
        };
    },
    methods: {
        submitPackage() {
            // You can implement the logic here to submit the selected package
            console.log('Custom package submitted:', {
                hotel: this.selectedHotel,
                flight: this.selectedFlight,
                guide: this.selectedGuide,
                plan: this.travelPlan
            });
        }
    }
};
</script>
  
<style scoped>
.custom-package {
    max-width: 800px;
    margin: 0 auto;
    padding: 20px;
}

.package-options .option {
    margin-bottom: 20px;
}

.package-summary button {
    padding: 10px 20px;
    background-color: #007bff;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
}

.package-summary button:hover {
    background-color: #0056b3;
}
</style>
  