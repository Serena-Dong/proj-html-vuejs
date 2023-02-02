<script>
export default {
    name: 'partnerships'
}
</script>

<template>
    <section>
        <div class="container">
            <div class="text">
                <h1>Some Brands We Work With</h1>
                <p>Quisque aliquet, libero consequat elementum convallis</p>
            </div>
            <div class="brands">
                <ul>
                    <li></li>
                </ul>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/css/scss/partials/_variables' as *;

.container {
    text-align: center;

    .text {
        h1 {
            font-size: 3rem;
        }

        p {
            color: $grey;
        }
    }

    .text>* {
        margin-bottom: 1rem;
    }
}
</style>