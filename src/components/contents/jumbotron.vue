<script>
export default {
    name: 'jumbotron'
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

                <form action=""></form>
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
    height: 400px;
    align-items: center;

    .presentation {
        width: 600px;
        border: 2px solid black;

        color: white;
        font-size: 1.5rem;

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
                background-color: $black;

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