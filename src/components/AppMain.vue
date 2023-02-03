<script>
import jumbotron from './contents/jumbotron.vue'
import card from './contents/card.vue'
import brands from './contents/brands.vue'
import contactCard from './contents/contactCard.vue'
import testimonials from './contents/testimonials.vue'
import campaign from './contents/campaign.vue'
import intern from './contents/intern.vue'
import resources from './contents/resources.vue'
import outro from './contents/outro.vue'


export default {
    name: 'AppMain',
    components: {
        jumbotron,
        card,
        brands,
        contactCard,
        testimonials,
        campaign,
        intern,
        resources,
        outro
    },
    emits: [
        'form-submit', 'name-submit', 'email-submit', 'phone-submit'
    ]

}
</script>

<template>
    <main>
        <jumbotron @name-submit="name - submit"></jumbotron>
        <card></card>
        <brands></brands>
        <contactCard></contactCard>
        <testimonials></testimonials>
        <campaign></campaign>
        <intern></intern>
        <resources></resources>
        <outro></outro>
    </main>
</template>

<style lang="scss" scoped>

</style>