<template>
    <div class="banner">
        <img src="/images/bannerr.png" alt="Logo">
        <div class="banner-text">
            <h1 class="banner-header">
                <span class="empower">EMPOWERING YOUR FUTURE WITH</span><br>
                <span class="cutting">CUTTING-EDGE TECHNOLOGY </span>
            </h1>
             <p class="banner-paragraph">
                To help your business grow. From  <br>
                software development to IT consulting,<br>
                we’ve got you covered
            </p>
            <div>
                <a href="#get-started" class="get-started-btn">Get Started</a>
            </div>  
        </div>
    </div>

</template>

<script>
    export default {
        name: 'Banner'
    }
</script>

<style scoped>
    .banner-header {
    font: bold;
    padding: 10px;
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
    text-align: center;
    padding: 5px;
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

@media (max-width: 768px) {
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

}
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

    }
</style>