<script>
import formSection from './formSection.vue'
export default {
    name: 'jumbotron',
    components: { formSection }
}
</script>

<template>
    <div class="jumbotron">
        <div class="container">
            <div class="row">
                <div class="presentation">
                    <h1>Unlock Your Online Growth Potential</h1>
                    <p>Online marketing to secure customer retention, leads and sales. We focus on the bigger picture.
                    </p>
                    <button class="white">
                        <a href="">
                            Our Services
                            <i class="fa-solid fa-arrow-right"></i>
                        </a>
                    </button>
                </div>

                <formSection></formSection>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../../assets/css/scss/partials/_variables' as *;

.jumbotron {
    height: 500px;
    background-image: url("../../assets/img/marketing-intro.jpg");
    background-repeat: no-repeat;
    background-size: cover;
}

.row {
    display: flex;
    height: 500px;
    align-items: center;

    .presentation {
        width: 550px;
        color: white;
        font-size: 1.5rem;
        margin-right: 5rem;

        .white {
            background-color: $white;
            border: $white;

            a {
                color: $black;

                .fa-arrow-right {
                    font-size: 1rem;
                    margin-left: 0.5rem;
                }
            }

            &:hover {
                background-color: rgba(255, 255, 255, 0);
                border: 1px solid $white;

                a {
                    color: $white;

                }
            }
        }

    }

    .presentation>* {
        margin-bottom: 2rem;
    }
}
</style>