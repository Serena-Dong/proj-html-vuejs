<script>
import jumbotron from './contents/jumbotron.vue'
import card from './contents/card.vue'
import brands from './contents/brands.vue'
import contactCard from './contents/contactCard.vue'
import testimonials from './contents/testimonials.vue'
import campaign from './contents/campaign.vue'
import awards from './contents/awards.vue'
import intern from './contents/intern.vue'
import resources from './contents/resources.vue'
import jumbotronB from './contents/jumbotronB.vue'


export default {
    name: 'AppMain',
    components: {
        jumbotron, card, brands, contactCard, testimonials, campaign, awards, intern, resources, jumbotronB
    }

}
</script>

<template>
    <jumbotron></jumbotron>
    <card></card>
    <brands></brands>
    <contactCard></contactCard>
    <testimonials></testimonials>
    <campaign></campaign>
    <awards></awards>
    <intern></intern>
    <resources></resources>
    <jumbotronB></jumbotronB>
</template>

<style lang="scss" scoped>

</style>