<script>
export default {
    name: 'btn',
    props: {
        text: String
    }
}
</script>

<template>

    <!-- BUTTON -->
    <button type="submit" class="ochre"><a href="">{{ text }}</a></button>

</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/_variables' as *;

.ochre {
    background-color: $ochre;
    border: $ochre;

    a {
        color: $white;
    }

    &:hover {
        background-color: #ffba31;

    }
}
</style>