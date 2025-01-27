<template>
    <div class="services-info">
        <h1 class="services-header">Services Information</h1>
        <p>
            Elevate your business with our innovative solutions! At Me<span class="metech-tech">Tech</span>, we provide cutting-edge services tailored to streamline your operations, enhance collaboration, and drive success. Let us help you achieve your goals fast and efficiently!
        </p>
    </div>

</template>

<script>
    export default {
        name: 'ServicesInfo'
    }
</script>

<style scoped>
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

.metech-tech {
    color: #007BFF;
}

@media (max-width: 768px) {

}

</style>