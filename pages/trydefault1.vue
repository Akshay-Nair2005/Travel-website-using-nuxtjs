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
    <div class="default-packages">
        <h1>Explore Kerala with Our Default Packages</h1>
        <div class="package-list">
            <div v-for="packag in packages" :key="packag.id" class="package">
                <h2>{{ packag.name }}</h2>
                <img src="./static/kerala.jpg" alt="#">
                <p class="package-description">{{ packag.description }}</p>
                <p><strong>Hotel:</strong> {{ packag.hotel }}</p>
                <p><strong>Flight:</strong> {{ packag.flight }}</p>
                <p><strong>Travel Guide:</strong> {{ packag.guide }}</p>
                <p><strong>Travel Plan:</strong> {{ packag.travelPlan }}</p>
                <button @click="bookPackage(package)">Book Now</button><br><br><br><br>
            </div>

        </div>
    </div>
</template>
  
<script>
export default {
    data() {
        return {
            packages: [
                {
                    id: 1,
                    name: 'Relaxing Retreat',
                    description: 'Indulge in a serene getaway in the heart of Kerala.',
                    hotel: 'Luxury Spa Resort',
                    flight: 'Flight A',
                    guide: 'Local Expert 1',
                    travelPlan: 'Enjoy leisurely walks by the backwaters and savor local cuisine.'
                },
                {
                    id: 2,
                    name: 'Adventure Expedition',
                    description: 'Embark on an exciting adventure through Kerala\'s rugged terrains.',
                    hotel: 'Adventure Lodge',
                    flight: 'Flight B',
                    guide: 'Local Expert 2',
                    travelPlan: 'Explore hiking trails, wildlife sanctuaries, and thrilling activities.'
                },
                {
                    id: 3,
                    name: 'Cultural Discovery',
                    description: 'Immerse yourself in Kerala\'s rich cultural heritage and traditions.',
                    hotel: 'Heritage Homestay',
                    flight: 'Flight C',
                    guide: 'Local Historian',
                    travelPlan: 'Visit ancient temples, witness traditional art forms, and experience local festivals.'
                },
                {
                    id: 4,
                    name: 'Backwater Bliss',
                    description: 'Unwind with a serene journey through Kerala\'s tranquil backwaters.',
                    hotel: 'Houseboat Retreat',
                    flight: 'Flight D',
                    guide: 'Local Navigator',
                    travelPlan: 'Cruise along the scenic waterways, enjoy fresh seafood, and witness breathtaking sunsets.'
                },
                {
                    id: 5,
                    name: 'Beach Paradise',
                    description: 'Relax on the pristine beaches of Kerala\'s coastline.',
                    hotel: 'Beachfront Resort',
                    flight: 'Flight E',
                    guide: 'Beach Enthusiast',
                    travelPlan: 'Sunbathe on golden sands, try water sports, and indulge in beachside dining.'
                }



                // Add more packages as needed
            ]
        };
    },
    methods: {
        bookPackage(selectedPackage) {
            // You can implement booking logic here
            console.log('Package booked:', selectedPackage);
        }
    }
};
</script>
  
<style scoped>
.default-packages {
    max-width: 800px;
    margin: 0 auto;
    padding: 20px;
    text-align: center;
}

.package-list {
    width: 100%;
    display: flex;
    /* justify-content: space-around; */
    flex-wrap: wrap;
    height: 35%;
}

.package-list img {
    width: 100%;
    height: 45%;
}

.package {
    max-width: 300px;
    margin: 20px;
    padding: 20px;
    border: 1px solid #ddd;
    border-radius: 8px;
    text-align: left;
}

.package h2 {
    margin-top: 0;
}

.package-description {
    font-style: italic;
    color: #777;
    margin-bottom: 10px;
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


* {
    margin: 0;
    padding: 0;
    /* box-sizing: border-box; */
    /* border: 2px solid red; */


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
</style>
  