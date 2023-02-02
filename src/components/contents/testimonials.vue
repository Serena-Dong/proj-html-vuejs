<script>
import btn from './button.vue'
export default {
    name: 'testimonials',
    components: { btn },
    data() {
        return {
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
                <div class="testimonial">
                    <div class="profile-pic">
                        <img src="../../assets/img/testimonials/case-studies-1.jpg" alt="">
                    </div>
                    <div class="profile-text">
                        <p>How Spaces attracted five million visitors by improving the content</p>

                        <h1>200%</h1>
                        <span>Higher revenue from digital</span>

                    </div>
                </div>
                <div class="testimonial">
                    <div class="profile-pic">
                        <img src="../../assets/img/testimonials/case-studies-4.jpg" alt="">
                    </div>
                    <div class="profile-text">
                        <p>Creativity helped Hemisfero to increase their brand reach vertically</p>

                        <h1>10x</h1>
                        <span>Sales increase with the same ad spend</span>

                    </div>
                </div>
                <div class="testimonial">
                    <div class="profile-pic">
                        <img src="../../assets/img/testimonials/case-studies-6.jpg" alt="">
                    </div>
                    <div class="profile-text">
                        <p>How DigitalBox used AI-powered data inisght to boost sales</p>

                        <h1>3-year</h1>
                        <span>Partnership with Avada Consultant</span>

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