<template>
    <nav class="nav">
        <div class="logo">
            <!--<p class="metech-logo">
                <span class="me">Me</span>
                <span class="tech">Tech</span>
            </p>-->
            <img src="/images/metechlogo.png" alt="Metech Logo" class="metech-logo">
        </div>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#contact" class="contact-class">Contact Us</a></li>
        </ul>
    </nav>
</template>


<script>
    export default {
        name: 'Menu'
    }
</script>


<style scoped>
  nav img {
    width: 100px;
    height: auto;
  }

    nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: rgb(255, 255, 255);
  width: 100%;
  padding: 1rem 0;
  height: 70px;
}

nav ul {
  list-style: none;
  padding: 0;
  display: flex;
  gap: 1rem;
}

nav a {
  text-decoration: none;
  color: #1714cf;
  padding-right: 10px;
}


/*.metech-logo {
        margin-left: 10px;
        font-weight: bold;        
    } */

.me {
        color: rgb(0, 0, 0);
    }

.tech {
        color: blue;
        font-weight: 200;
    }

    ul li a {
    font-weight: bold;
    font-size: large;    
}

.contact-class {
  padding: 10px;
  background-color: rgb(37, 77, 255);
  color: white;
  border-radius: 20px;
  margin: 10px;
}

@media (max-width: 768px) {
    .nav {
    flex-wrap: wrap; /* Allow wrapping if needed */
    padding: 1rem; /* Adjust padding for smaller screens */
  }
  .nav ul {
    order: 2; /* Ensure links stay on the right */
    flex: 1; /* Push links to the right */
    justify-content: flex-end; /* Align links to the right */
  }

  .nav ul li {
    margin-left: 0.5rem; /* Slightly smaller spacing on mobile */
  }
  .logo {
    order: 1; /* Ensure logo stays on the left */
    flex: 1; /* Push logo to the left */
  }


}
</style>