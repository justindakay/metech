<template>
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
        name: 'Footer',

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

@media (max-width: 768px) {
  .footer {
        padding: 15px;
    }
}

@media (max-width: 480px) {
  .footer {
        padding: 10px;
    }
}
</style>