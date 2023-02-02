<script>
import jumbotron from './contents/jumbotron.vue'
import card from './contents/card.vue'
import partnerships from './contents/partnerships.vue'


export default {
    name: 'AppMain',
    components: {
        jumbotron, card, partnerships
    }

}
</script>

<template>
    <jumbotron></jumbotron>
    <card></card>
    <partnerships></partnerships>
</template>

<style lang="scss" scoped>

</style>