<script>
import jumbotron from './contents/jumbotron.vue'
import card from './contents/card.vue'
import brands from './contents/brands.vue'


export default {
    name: 'AppMain',
    components: {
        jumbotron, card, brands
    }

}
</script>

<template>
    <jumbotron></jumbotron>
    <card></card>
    <brands></brands>
</template>

<style lang="scss" scoped>

</style>