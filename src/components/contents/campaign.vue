<script>
import { mainData } from '../../data/data'

import btn from './button.vue'
export default {
    name: 'campaign',
    components: { btn },
    data() {
        return {
            mainData,
            text: 'Why Work With Us'
        }
    }
}
</script>

<template>

    <!-- CAMPAIGN  -->

    <section>
        <div class="container">

            <!-- INTRO CAMPAIGN -->
            <div class="row">
                <div class="text-col">
                    <h1>We Boost Our Clients' Bottom Line by Optimizing Their Growth Potential.</h1>
                    <p>Modi dolores voluptate quas quaerat
                        ipsum adipisci neque ipsam beatae impedit nihil obcaecati iusto, qui quasi.</p>
                    <btn :text="text"></btn>
                </div>
                <div class="img-col">
                    <img src="../../assets/img/b-roll/we-boost-our-clients.jpg" alt="">
                </div>
            </div>

            <!-- MAIN CAMPAIGN -->
            <div class="row">

                <!-- LEFT SIDE -->
                <div class="text-col">
                    <div class="text">
                        <p class="bigger">We Build Relationship</p>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Enim saepe vel velit animi, minus
                            error!</p>
                    </div>
                    <div class="text">
                        <p class="bigger">Priorietary Processes</p>
                        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Exercitationem et id nihil?</p>
                    </div>
                </div>

                <!-- RIGHT SIDE -->
                <div class="text-col">
                    <div v-for="point in mainData.campaign" class="main-point">
                        <div class="point-img">
                            <img :src="point.img" alt="">
                        </div>
                        <div class="point-details">
                            <p id="point-name">{{ point.name }}</p>
                            <p>{{ point.detail }}</p>
                        </div>
                    </div>
                </div>
            </div>

            <!-- AWARDS -->
            <div class="awards">
                <div class="title">
                    <h2>Awards</h2>
                </div>
                <ul>
                    <li v-for="award in mainData.awards">
                        <img :src="award.img" alt="">
                        <p>{{ award.name }}</p>
                        <p>{{ award.year }}</p>
                    </li>
                </ul>
            </div>
        </div>

    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables' as *;

section {
    background-color: $white-2;
}

.container {
    height: 1700px;

    .row {
        display: flex;
        justify-content: space-around;
        align-items: center;
        padding-top: 6rem;

        .img-col {
            width: 600px;

            img {
                border-radius: 1rem;
            }
        }

        .text-col {

            margin-top: 3rem;
            display: block;
            width: 400px;
            font-size: 1.3rem;

            h1 {
                font-size: 2.5rem;
            }

            p {
                font-size: 1.1rem;
                line-height: 2.2rem;
            }

            .text {
                margin-bottom: 4rem;
            }

            .bigger {
                font-size: 2rem;
                margin-bottom: 1rem;
            }
        }

        .text-col>*,
        .text>* {
            margin-bottom: 2rem;
        }
    }
}

.main-point {
    display: flex;
    align-items: center;
    height: 100px;

    .point-img {
        margin-right: 1rem;
    }

    #point-name {
        font-size: 1.5rem;
    }
}

.awards {
    text-align: center;
    margin-top: 4rem;

    ul {
        display: flex;
        justify-content: space-around;

        li {

            img {
                width: 200px;
            }

            p {
                margin-bottom: 1rem;
            }
        }
    }
}
</style>