<script>
export default {
    name: 'btn',
    props: {
        text: String
    }
}
</script>

<template>
    <button class="transparent"><a href="">{{ text }}</a></button>
</template>

<style lang="scss" scoped>
@use '../../assets/css/scss/partials/_variables' as *;

.transparent {
    background-color: rgba(255, 136, 0, 0.313);
    border: rgba(255, 136, 0, 0.313);

    a {
        color: $ochre;
    }

    &:hover {
        background-color: $ochre;

        a {
            color: $white;

        }
    }
}
</style>