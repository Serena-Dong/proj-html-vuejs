<script>
import { mainData } from '../../data/data';

import btn from './button.vue'
export default {
    name: 'resources',
    components: { btn },
    data() {
        return {
            mainData,
            text: 'Explore All Resources'
        }
    }
}
</script>

<template>

    <!-- RESOURCES -->

    <section>
        <div class="container">
            <div class="row">

                <!-- TITLE -->
                <div class="text-col">
                    <h1>Marketing Resources: Insider Advice on How to Increase Online Sales</h1>
                </div>

                <!-- BUTTON -->
                <div class="btn-col">
                    <btn :text="text"></btn>
                </div>
            </div>

            <!-- RESOURCES POINTS -->
            <ul>
                <li v-for="resource in mainData.resources">

                    <!-- IMG -->
                    <img class="hover-orange" :src="resource.img" alt="">

                    <!-- TEXT -->
                    <p>{{ resource.text }}</p>

                </li>
            </ul>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables' as *;

section {
    background-color: $white-2;
}

.container {
    height: 750px;


}

.row {
    height: 300px;
    display: flex;
    justify-content: space-around;
    align-items: flex-end;
    padding-bottom: 4rem;


    .text-col {
        width: 400px;

        h1 {
            font-size: 2rem;
        }
    }

    .btn-col {
        width: 200px;
    }
}

ul {
    display: flex;
    justify-content: center;

    li {
        width: 300px;

        img {
            margin-bottom: 1rem;
        }

        p {
            font-size: 1.5rem;
        }
    }
}
</style>