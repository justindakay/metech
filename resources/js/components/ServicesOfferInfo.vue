<template>
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

</template>

<script>
    export default {
        name: 'ServicesOfferInfo'
    }
</script>

<style scoped>
        .services-offer-info {
    background-color: rgb(138, 182, 202);
    align-items: center;
    display: flex;
    justify-content: space-around;
    padding: 2rem 0;
    gap: 40px;
}

.services-offer-info img {
    margin: 0 auto;
    width: 100%;
    max-width: 150px;
    height: auto;
}

.web-text {
    text-align: center;
    margin-top: 10px;
    color: white;
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

@media (max-width: 768px) {
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
}

@media (max-width: 480px) {
    .services-offer-info {
        gap: 10px;
    }

    .services-webdev {
        width: 100%;
    }

}
</style>