<template>
    <div>
        <Menu />
        <Banner />
        <ServicesInfo />
        <ServicesOfferInfo />
        <Footer />
    </div>
</template>


<script>

import Menu from './Menu.vue';
import Banner from './Banner.vue';
import ServicesInfo from './ServicesInfo.vue';
import ServicesOfferInfo from './ServicesOfferInfo.vue';
import Footer from './Footer.vue';



    export default {
        mounted() {
            console.log('Component mounted.')
        },
        name: 'Main',
        components: {
            Menu,
            Banner,
            ServicesInfo,
            ServicesOfferInfo,
            Footer
        }



      
    }
</script>



<style scoped>

/* Mobile Responsiveness */
@media (max-width: 768px) {   
}

/* Mobile responsiveness for very small screens */
@media (max-width: 480px) {   
}
</style> 