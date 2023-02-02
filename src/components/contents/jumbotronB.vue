<script>
import formSection from './formSection.vue'
export default {
    name: 'jumbotronB',
    components: {
        formSection
    }
}
</script>

<template>
    <section>
        <div class="container">
            <div class="row">
                <div class="text-col">
                    <h1>Let's Make Things Happen</h1>
                    <br>
                    <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Hic consequuntur consectetur deserunt.
                        Integer consectetur</p>
                    <div></div>
                    <p>
                        <i class="smaller">"The team at Avda Marketing Consultant is fabulous. They helped us unlock our
                            potential
                            online
                            and offline. We have experienced year on year groth due to their progressive approch"
                        </i>
                    </p>
                    <br>
                    <h4>George Anderson</h4>
                    <span>Digitalbox CEO</span>
                </div>
                <formSection></formSection>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables' as *;

section {
    background-color: $black;
}

.container {
    height: 700px;

    .row {
        display: flex;
        height: 600px;
        justify-content: center;
        gap: 10%;

        .text-col {
            margin-top: 6rem;

            width: 500px;
            color: $white;

            font-size: 1.2rem;
            line-height: 2rem;

            div {
                width: 80px;
                height: 2px;
                background-color: $grey;
                margin: 1.5rem 0 1.5rem;
                border-radius: 1rem;
            }

            h1 {
                font-size: 3rem;
                line-height: 4rem;
            }

            .smaller {
                font-size: 1rem
            }
        }

    }
}
</style>