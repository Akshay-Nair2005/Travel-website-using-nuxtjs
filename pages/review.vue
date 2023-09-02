<template>
    <div class="body">
        <header>
            <h1>Explore and Discover - Travel Reviews</h1>
        </header>

        <div class="review-container" id="reviewContainer">
            <!-- Existing reviews will be displayed here -->
            <div v-for="(review, index) in reviews" :key="index" class="review">
                <h2>{{ review.title }}</h2>
                <p><strong>Review by {{ review.author }}</strong></p>
                <p>{{ review.content }}</p>
                <br>
                <div>
                    <button :class="{ active: review.likeActive }" @click="toggleLike(index)">
                        👍 {{ review.likes }}
                    </button>
                    <button :class="{ active: review.dislikeActive }" @click="toggleDislike(index)">
                        👎 {{ review.dislikes }}
                    </button>
                    <br><br>
                    <input type="text" v-model="newComments[index]" placeholder="Write a comment...">
                    <br> <br>
                    <button @click="addComment(index)">Add Comment</button>
                    <br><br>
                    <ul>
                        <li v-for="comment in review.comments" :key="comment">{{ comment }}</li>
                    </ul>
                </div>
            </div>
        </div>

        <div class="review-container add-review-container">
            <h2>Add Your Review</h2>
            <form @submit.prevent="submitReview">
                <label for="reviewTitle">Title:</label>
                <input v-model="newReview.title" type="text" id="reviewTitle" required>

                <label for="reviewAuthor">Your Name:</label>
                <input v-model="newReview.author" type="text" id="reviewAuthor" required>

                <label for="reviewContent">Review:</label>
                <textarea v-model="newReview.content" id="reviewContent" required></textarea>

                <button type="submit">Submit Review</button>
            </form>
        </div>
    </div>
</template>
  
<style scoped>
/* Your CSS styles here */
.body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    margin: 0;
    padding: 0;
    background-color: azure;
}

header {
    background-color: rgb(3, 34, 90);
    color: #fff;
    text-align: center;
    padding: 1rem;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
}

.review-container {
    max-width: 800px;
    margin: 0 auto;
    padding: 1rem;
}

.review {
    margin-bottom: 1.5rem;
    border: 1px solid #ccc;
    padding: 1rem;
    border-radius: 5px;
    background-color: #fff;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.review h2 {
    margin-top: 0;
}

.review p {
    margin-bottom: 0.5rem;
}

.review-container.add-review-container {
    background-color: #f2f2f2;
    padding: 1rem;
    border-radius: 5px;
    margin-bottom: 2rem;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    border: 2px solid rgb(3, 34, 90);
}

.review-container.add-review-container h2 {
    margin-top: 0;
}

.review-container.add-review-container form {
    display: flex;
    flex-direction: column;
}

.review-container.add-review-container label {
    margin-bottom: 0.5rem;
}

.review-container.add-review-container input[type="text"],
.review-container.add-review-container textarea {
    padding: 0.5rem;
    margin-bottom: 1rem;
    border: 1px solid #ccc;
    border-radius: 3px;
    font-family: Arial, sans-serif;
}

.review-container.add-review-container button[type="submit"] {
    padding: 0.5rem 1rem;
    background-color: rgb(3, 34, 90);
    color: #fff;
    border: none;
    border-radius: 3px;
    cursor: pointer;
    font-size: 1rem;
    font-family: Arial, sans-serif;
}

/* Additional styles for review buttons and comments */
.review button {
    background-color: rgb(3, 34, 90);
    color: #fff;
    border: none;
    padding: 0.25rem 0.5rem;
    margin-right: 0.5rem;
    border-radius: 3px;
    cursor: pointer;
}

.review span {
    margin-right: 1rem;
}

.review input[type="text"] {
    width: 100%;
}

.review button[type="submit"] {
    width: 100px;
    margin-top: 1rem;
}

.review ul {
    list-style: none;
    margin: 0;
    padding: 0;
}

.review li {
    margin-bottom: 0.5rem;
    border-bottom: 1px solid #ccc;
    padding-bottom: 0.25rem;
}
</style>
  
<script>
export default {
    data() {
        return {
            reviews: [
                {
                    title: "Breathtaking Beach Paradise - Maldives",
                    author: "WanderlustExplorer",
                    content: "The Maldives is a true slice of heaven on Earth! Crystal-clear turquoise waters...",
                    likes: 0,
                    dislikes: 0,
                    likeActive: false,
                    dislikeActive: false,
                    comments: []
                },
                {
                    title: "Cultural Wonderland - Kyoto, Japan",
                    author: "CultureVulture",
                    content: "Kyoto is a city that effortlessly blends tradition and modernity...",
                    likes: 0,
                    dislikes: 0,
                    likeActive: false,
                    dislikeActive: false,
                    comments: []
                },
                // Add more reviews here
            ],
            newReview: {
                title: "",
                author: "",
                content: ""
            },
            newComments: []
        };
    },
    methods: {
        submitReview() {
            if (
                this.newReview.title.trim() === "" ||
                this.newReview.author.trim() === "" ||
                this.newReview.content.trim() === ""
            ) {
                alert("Please fill in all fields.");
                return;
            }

            this.reviews.push({
                title: this.newReview.title,
                author: this.newReview.author,
                content: this.newReview.content,
                likes: 0,
                dislikes: 0,
                likeActive: false,
                dislikeActive: false,
                comments: []
            });

            this.newReview = {
                title: "",
                author: "",
                content: ""
            };
        },
        toggleLike(index) {
            const review = this.reviews[index];
            if (!review.likeActive) {
                review.likes++;
                review.likeActive = true;
                if (review.dislikeActive) {
                    review.dislikes--;
                    review.dislikeActive = false;
                }
            } else {
                review.likes--;
                review.likeActive = false;
            }
        },
        toggleDislike(index) {
            const review = this.reviews[index];
            if (!review.dislikeActive) {
                review.dislikes++;
                review.dislikeActive = true;
                if (review.likeActive) {
                    review.likes--;
                    review.likeActive = false;
                }
            } else {
                review.dislikes--;
                review.dislikeActive = false;
            }
        },
        addComment(index) {
            if (this.newComments[index].trim() === "") {
                alert("Please enter a valid comment.");
                return;
            }

            this.reviews[index].comments.push(this.newComments[index]);
            this.newComments[index] = "";
        }
    }
};
</script>