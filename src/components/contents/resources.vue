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
    <section>
        <div class="container">
            <div class="row">
                <div class="text-col">
                    <h1>Marketing Resources: Insider Advice on How to Increase Online Sales</h1>
                </div>
                <div class="btn-col">
                    <btn :text="text"></btn>
                </div>
            </div>
            <ul>
                <li v-for="resource in mainData.resources">
                    <img :src="resource.img" alt="">
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