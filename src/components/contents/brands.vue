<script>
import { mainData } from '../../data/data'

export default {
    name: 'brands',
    data() {
        return {
            mainData,
        }
    }
}
</script>

<template>
    <section>

        <!-- BRANDS -->

        <div class="container">
            <div class="text">
                <h1>Some Brands We Work With</h1>
                <p>Quisque aliquet, libero consequat elementum convallis</p>
            </div>
            <div class="brands">
                <ul v-for="brand in mainData.brands.img">
                    <li><a href="">
                            <img :src="brand" alt="">
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/_variables' as *;

.container {
    text-align: center;
    margin-bottom: 6rem;


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

    .brands {
        display: flex;
    }
}
</style>