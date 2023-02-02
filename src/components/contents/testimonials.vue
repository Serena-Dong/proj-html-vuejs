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
    <section>
        <div class="container">
            <div class="title">
                <h1>Trusted By Leading Organisation</h1>
            </div>
            <div class="row">
                <div v-for="testimonial in mainData.testimonials" class="testimonial">
                    <div class="profile-pic">
                        <img :src="testimonial.img" alt="">
                    </div>
                    <div class="profile-text">
                        <p>{{ testimonial.text }}</p>

                        <h1>{{ testimonial.point }}</h1>
                        <span>{{ testimonial.detail }}</span>

                    </div>
                </div>
            </div>
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