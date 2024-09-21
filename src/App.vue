

<script setup>
  import Section1 from './components/Section1.vue'
</script>

<template>
  <header>
        <h1>Mini Blog</h1>
        <nav>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Politics</a></li>
                <li><a href="#">Tech</a></li>
                <li><a href="#">Entertainment</a></li>
                <li><a href="#">Travel</a></li>
                <li><a href="#">Sports</a></li>
            </ul>
        </nav>
    </header>

    <Section1/>
</template>

<style scoped>
  header 
  {
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

</style>
