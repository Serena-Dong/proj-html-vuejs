<script>
import { mainData } from '../../data/data'
export default {
    name: 'intern',
    data() {
        return {
            mainData
        }
    }
}
</script>

<template>

    <!-- INTERN -->

    <section>
        <div class="container">
            <div class="row">

                <!-- IMG  -->
                <div class="img-col">
                    <img :src="mainData.intern.img" alt="">
                </div>

                <!-- TEXT -->
                <div class="text-col">
                    <p>"{{ mainData.intern.text }}"</p>
                    <p>{{ mainData.intern.name }}</p>
                    <span>{{ mainData.intern.role }}</span>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables' as *;

.container {
    .row {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 600px;
        gap: 8%;


        .img-col {
            width: 400px;

            img {
                border-radius: 1rem;
            }
        }

        .text-col {
            width: 300px;

            p {
                font-size: 1.2rem;
                line-height: 2rem;
                margin-top: 1.5rem;
            }
        }


    }
}
</style>