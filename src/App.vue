<template>

<Navbar />
<router-view />
<Card />
<Footer />
<AboutView />
</template>

<script>

import Navbar from './components/Navbar.vue'
import Card from './components/Card.vue';
import Footer from './components/Footer.vue';
import AboutView from './views/AboutView.vue';

export default {
    components: {
    Navbar,
    Card,
    Footer,
    AboutView
},
}
</script>


<style></style>
