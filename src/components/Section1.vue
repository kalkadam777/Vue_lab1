<script setup>
import { ref } from 'vue'

// name: 'Section1',
// defineProps({
//   msg: String,
// })

const count = ref(0)
</script>

<template>
    <div class="container">
        <section class="featured-posts">
            <article class="post large-post">
                <img src="../assets/image1.png" alt="Large Post Image" class="large_pic">
                <div class="post-content">
                    <h2>The AI Magically Removes Moving Objects from Videos</h2>
                    <div class="meta">July 19, 2019</div>
                </div>
            </article>
            <div class="small-posts">
                <article class="post">
                    <img src="../assets/image2.png" alt="Small Post Image">
                    <div class="post-content">
                        <h2>The 20 Biggest Fintech Companies in America 2019</h2>
                        <div class="meta">July 19, 2019</div>
                    </div>
                </article>

                <article class="post">
                    <img src="../assets/image3.png" alt="Small Post Image">
                    <div class="post-content">
                        <h2>How to Leverage Machine Learning in Your Business</h2>
                        <div class="meta">July 20, 2019</div>
                    </div>
                </article>
            </div>
        </section>

        <section class="recent-posts">
            <h3>Recent Posts</h3>
            <div class="grid">
                <article class="post">
                    <img src="../assets/im4.png" alt="Post Image">
                    <div class="post-content">
                        <h2>The Future of Quantum Computing</h2>
                        <div class="meta">July 21, 2019</div>
                    </div>
                </article>

                <article class="post">
                    <img src="../assets/im5.png" alt="Post Image">
                    <div class="post-content">
                        <h2>Advancements in Renewable Energy Technologies</h2>
                        <div class="meta">July 22, 2019</div>
                    </div>
                </article>

                <article class="post">
                    <img src="../assets/im6.png" alt="Post Image">
                    <div class="post-content">
                        <h2>The Impact of Social Media on Society</h2>
                        <div class="meta">July 23, 2019</div>
                    </div>
                </article>
            </div>
        </section>
    </div>

</template>

<style scoped>

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            background-color: #f4f4f4;
            color: #333;
        }

        header {
            background-color: #fff;
            padding: 20px;
            border-bottom: 1px solid #ddd;
            position: relative;
        }

        header h1 {
            font-size: 1.5em;
        }

        nav {
            position: absolute;
            top: 50%;
            right: 20px;
            transform: translateY(-50%);
        }

        nav ul {
            list-style: none;
            display: flex;
        }

        nav ul li {
            margin-left: 20px;
        }

        nav ul li a {
            text-decoration: none;
            color: #333;
            font-weight: bold;
        }

        .container {
            max-width: 1200px;
            margin: 40px auto;
            padding: 0 20px;
        }

        .featured-posts {
            display: grid;
            grid-template-columns: 2fr 1fr;
            grid-gap: 20px;
        }

        .featured-posts .large-post {
            position: relative;
        }

        .featured-posts .small-posts {
            display: grid;
            grid-template-rows: repeat(2, 1fr);
            grid-gap: 20px;
        }

        
        .recent-posts .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .recent-posts h3 {
            margin-top: 20px;
        }

        
        .post {
            position: relative;
            overflow: hidden;
            border-radius: 8px;
        }

        .post img {
            width: 100%;
            height: auto;
            display: block;
        }

        .post-content {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            padding: 20px;
            background: linear-gradient(to top, rgba(0,0,0,0.8), transparent);
            color: #fff;
        }

        .post-content h2 {
            font-size: 1.2em;
            margin-bottom: 5px;
        }

        .post-content .meta {
            font-size: 0.9em;
            color: #ccc;
        }

        
        .post:hover img {
            transform: scale(1.05);
            transition: transform 0.3s ease;
        }

        
   
</style>
