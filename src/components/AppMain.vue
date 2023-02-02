<script>
import jumbotron from './contents/jumbotron.vue'
import section from './contents/section.vue'
import partnerships from './contents/partnerships.vue'


export default {
    name: 'AppMain',
    components: {
        jumbotron, section, partnerships
    }

}
</script>

<template>
    <jumbotron></jumbotron>
    <section></section>
    <partnerships></partnerships>
</template>

<style lang="scss" scoped>

</style>