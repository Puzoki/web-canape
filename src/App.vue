<template>
    <top></top>
    <services></services>
    <about></about>
    <promo></promo>
    <coaches></coaches>
    <reviews></reviews>
    <news></news>
    <bottom></bottom>
</template>

<script>
import top from './components/Top.vue'
import services from './components/Services.vue'
import about from './components/About.vue'
import promo from './components/Promo.vue'
import coaches from './components/Coaches.vue'
import reviews from './components/Reviews.vue'
import news from './components/News.vue'
import bottom from './components/Bottom.vue'


export default {
    name: "#app",
    components: {
        top,
        services,
        about,
        promo,
        coaches,
        reviews,
        news,
        bottom,
    },
}
</script>

<style scoped></style>
