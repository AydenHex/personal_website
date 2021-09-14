<template>
    <div class="hero">
        <Navbar />
        <div class="main__content">
            <Sidebar />            
            <HeroContent />
        </div>
        <Signature />
    </div>
</template>

<script>
import Navbar from "./Navbar/Navbar.vue";
import HeroContent from "./HeroContent.vue";
import Sidebar from "./Sidebar.vue";
import Signature from "./Signature.vue";
export default {
    components: {Navbar, HeroContent, Sidebar, Signature}
}
</script>

<style>
    .hero {
        background-color: var(--main-hero-bg);
        width: 100vw;
        height: 100vh;
        display: flex;
        flex-direction: column;
    }

    .main__content {
        display: flex;
    }
</style>