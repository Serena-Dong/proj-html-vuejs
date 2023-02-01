<script>
export default {
    name: 'AppFooter'
}
</script>

<template>
    <div class="container">
        <div class="footer-top"></div>
        <div class="footer-bottom"></div>
    </div>
</template>

<style lang="scss" scoped>
.container {
    height: 600px;
    border: 2px solid black;

    .footer-top {
        height: 400px;
        border: 2px solid black;

    }

    .footer-bottom {
        height: 200px;
        border: 2px solid black;
    }
}
</style>