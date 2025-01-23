<template>
    <nav class="nav">
        <div class="logo">
            <p class="metech-logo">
                <span class="me">Me</span>
                <span class="tech">Tech</span>
            </p>
        </div>
    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#contact">Contact Us</a></li>
    </ul>
    </nav>

    <div class="banner">
        <img src="/images/bannerr.png" alt="Logo">
        <div class="banner-text">
            <h1 class="banner-header">
                <span class="empower">EMPOWERING YOUR FUTURE WITH</span><br>
                <span class="cutting">CUTTING-EDGE TECHNOLOGY </span>
            </h1>
             <p class="banner-paragraph">
                To help your business grow. From software <br>
                development to IT consulting,<br>
                we’ve got you covered
            </p>
            <div>
                <a href="#get-started" class="get-started-btn">Get Started</a>
            </div>  
        </div>
    </div>
    <div class="services-info">
        <h1 class="services-header">Services Information</h1>
        <p>
            Elevate your business with our innovative solutions! At Me<span class="metech-tech">Tech</span>, we provide cutting-edge services tailored to streamline your operations, enhance collaboration, and drive success. Let us help you achieve your goals fast and efficiently!
        </p>
    </div>
    <div class="services-offer-info">
        <div class="service-webdev">
            <img src="/images/web-development.png" alt="Web Development image">
            <div class="web-text">
                <h1 class="header-web">Web Development</h1>
                <p class="web-paragraph">
                    Transform your ideas into dynamic, <br>
                     user-friendly websites with our expert<br>
                       web development services
                </p>
            </div>
        </div>
        <div class="service-webdev">
            <img src="/images/app-development.png" alt="Mobile Development image">
            <div class="web-text">
                <h1 class="header-mobile">Mobile Development</h1>
                <p class="mobile-paragraph">
                    We deliver innovative, user-friendly mobile <br>
                     apps designed to bring your ideas to <br>
                      life and connect with your audience."
                </p>
            </div>
        </div>
        <div class="service-webdev">
            <img src="/images/project-management.png" alt="Project Management image">
            <div class="web-text">
                <h1 class="header-project">Project Management</h1>
                <p class="project-paragraph">
                    Our expert project management services ensure <br>
                     efficient collaboration and successful  <br>
                     project delivery every time.
                </p>
            </div>
        </div>
    </div>

    <footer class="footer">
        <div class="social-links">
      <a
        v-for="(link, index) in socialLinks"
        :key="index"
        :href="link.url"
        :title="link.name"
        target="_blank"
        class="social-icon"
      >
        <img :src="link.icon" :alt="link.name" />
      </a>
    </div>
        <p> All rights reserved | 
            <a href="/privacy-policy" title="Privacy Policy">Privacy Policy</a> | 
            <a href="/terms-and-conditions" title="Terms and Conditions">Terms and Conditions</a>
        </p>
        <p>Copyright &copy; 2025 MeTech.</p>
    </footer>
</template>


<script>
    export default {
        mounted() {
            console.log('Component mounted.')
        },

        data() {
    return {
      socialLinks: [
        { name: "Facebook", url: "https://facebook.com", icon: "/icons/facebook.svg" },
        { name: "Twitter", url: "https://twitter.com", icon: "/icons/twitter.svg" },
        { name: "Instagram", url: "https://instagram.com", icon: "/icons/instagram.svg" },
        { name: "LinkedIn", url: "https://linkedin.com", icon: "/icons/linkedin.svg" },
      ],
    };
  },
    }
</script>



<style scoped>
.metech-logo {
        margin-left: 10px;
        font-weight: bold;        
    }

.me {
        color: rgb(0, 0, 0);
    }

.tech {
        color: blue;
        font-weight: 200;
    }


.banner-header {
    font: bold;
    padding: 10px;
}   

.cutting {
    color: aquamarine;
}

    .get-started-btn {
    display: inline-block;
    background-color: #007BFF; /* Blue color */
    color: white;
    padding: 15px 30px;
    font-size: 18px;
    font-weight: bold;
    text-decoration: none;
    border-radius: 5px;
    margin-top: 20px;
    transition: background-color 0.3s;
}

.get-started-btn:hover {
    background-color: #0056b3; /* Darker blue on hover */
}

nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: rgb(255, 255, 255);
  width: 100%;
  padding: 1rem 0;
}
.logo img   {
    height: 50px;
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

ul li a {
    font-weight: bold;
    font-size: large;    
}

.banner {
    width: 100%;
    position: relative;
    align-items: center;
    display: flex;
    justify-content: space-between;
}

.banner img {
    width: 100%;
    height: auto; 
    max-width: 100%;
    margin: 0 auto;
    display: block;
}

.banner-text {
    flex: 0;
    align-items: flex-start;
    position: absolute;
   /* top: 40%; /* Adjust vertical position */
   /* left: 15%; /* Adjust horizontal position */
   /* transform: translate(-50%, -50%); /* Center the text */
    color: white;
    font-size: 30px; /* Adjust font size */
    font-weight: bold; /* Optional */
    margin: 10px;
    padding-left: 10px;
    text-align: center;   
}
.banner-paragraph {
    font-size: 20px;
}

.services-info {
    justify-content: center;
    align-items: center;
    text-align: center;
    background-color: #ffffff;
    margin: 30px;
}
.services-info p {
    font-size: 20px;
}

.services-header {
    font-size: 40px;
    color: #007BFF;
}
.metech-me {
    color: #007BFF;
}
.metech-tech {
    color: #007BFF;
}

.services-offer-info {
    background-color: rgb(138, 182, 202);
    align-items: center;
    display: flex;
    justify-content: space-around;
    padding: 2rem 0;
    gap: 40px;
}

.services-webdev {
    position: relative;
    text-align: center;
    width: 250px; /* Set a fixed width for the container */
    height: 350px; /* Set a fixed height for the container */
}

.web-text {
    text-align: center;
    margin-top: 10px;
    color: white;
}

.services-offer-info img {
    margin: 0 auto;
    width: 100%;
    max-width: 150px;
    height: auto;
}

.footer {
    background-color: rgb(203, 247, 247);
    text-align: center;
    bottom: 0;
    width: 100%;
    padding: 20px;
}

.social-links {
  display: flex;
  justify-content: center;
  gap: 20px;
}

.social-icon img {
  width: 30px;
  height: 30px;
}

.header-web, .header-mobile, .header-project {
    font-size: 20px;
    margin: 5px;
    color: rgb(51, 8, 247);
}

.web-paragraph, .mobile-paragraph, .project-paragraph {
    white-space: normal;
    text-align: center;
    color: black;
}


/* Mobile Responsiveness */
@media (max-width: 768px) {
    .nav {
    flex-wrap: wrap; /* Allow wrapping if needed */
    padding: 1rem; /* Adjust padding for smaller screens */
  }

  .logo {
    order: 1; /* Ensure logo stays on the left */
    flex: 1; /* Push logo to the left */
  }

  .nav ul {
    order: 2; /* Ensure links stay on the right */
    flex: 1; /* Push links to the right */
    justify-content: flex-end; /* Align links to the right */
  }

  .nav ul li {
    margin-left: 0.5rem; /* Slightly smaller spacing on mobile */
  }


  .banner-text {
        font-size: 24px; /* Smaller font size */
        padding-left: 5px; /* Adjust padding */
        margin: 5px; /* Reduce margin */
    }

    .banner-header {
        font-size: 26px; /* Adjust header font size */
    }
    .empower, .cutting {
        font-size: 18px; /* Adjust font size for span */
    }

    .banner-text p {
        font-size: 14px;
    }

    .get-started-btn {
        font-size: 18px; /* Adjust button text size */
        padding: 12px 24px; /* Adjust padding for button */
    }

    .services-offer-info {
        flex-direction: column;
        gap: 20px;
        padding: 1rem;
    }

    .services-webdev {
        width: 80%;
        height: auto;
    }

    .services-offer-info img {
        max-width: 100px;
    }

    .header-web, .header-mobile, .header-project {
        font-size: 18px;
    }

    .footer {
        padding: 15px;
    }
}

/* Mobile responsiveness for very small screens */
@media (max-width: 480px) {
    .banner-text {
        left: 5%;
        width: 90%;
    }

    .banner-header {
        font-size: 20px;
    }

    .banner-text p {
        font-size: 12px;
    }

    .get-started-btn {
        font-size: 14px;
        padding: 10px 20px;
    }

    .services-offer-info {
        gap: 10px;
    }

    .services-webdev {
        width: 100%;
    }

    .footer {
        padding: 10px;
    }
}
</style>