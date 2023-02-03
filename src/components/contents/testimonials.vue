<script>
import { mainData } from '../../data/data';

import btn from './button.vue';
export default {
    name: 'testimonials',
    components: { btn },
    data() {
        return {
            mainData,
            text: 'Read More Case Studies'
        }
    }
}
</script>

<template>

    <!-- TESTIMONIALS -->

    <section>
        <div class="container">

            <!-- TITLE -->
            <div class="title">
                <h1>Trusted By Leading Organisation</h1>
            </div>
            <div class="row">

                <!-- TESTIMONIAL CARD -->
                <div v-for="testimonial in mainData.testimonials" class="testimonial">

                    <!-- IMG -->
                    <div class="profile-pic">
                        <img class="hover-orange" :src="testimonial.img" alt="">
                    </div>

                    <!-- TEXT -->
                    <div class="profile-text">
                        <p>{{ testimonial.text }}</p>

                        <h1>{{ testimonial.point }}</h1>
                        <span>{{ testimonial.detail }}</span>

                    </div>
                </div>
            </div>
            <!-- BUTTON -->
            <div class="button">
                <btn :text="text"></btn>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables' as *;

h1 {
    font-size: 3rem;
}

p {
    font-size: 1.8rem;
    margin-bottom: 1.5rem;
}


.container {
    height: 900px;
    margin-bottom: 5rem;


    .title {
        text-align: center;
        margin-bottom: 4rem;
    }

    .row {
        display: flex;
        justify-content: space-around;
        margin-bottom: 3rem;

        .testimonial {
            width: 350px;
            height: 650px;

            .profile-pic {
                width: 350px;
                margin-bottom: 2rem;
            }

            .profile-text {
                width: 350px;
            }
        }
    }

    .button {
        text-align: center;
    }
}
</style>