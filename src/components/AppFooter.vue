<script>
import { footerData } from '../data/data';
export default {
    name: 'AppFooter',
    data() {
        return {
            footerData
        }
    }
}
</script>

<template>
    <div class="container">
        <div class="footer-top">
            <div class="row">
                <div class="col">
                    <!-- TEXT -->
                    <p>Grow Your Online Business Strategically, and Improve Customer Retention.</p>
                    <!-- SOCIALS -->
                    <div class="socials">
                        <ul>
                            <li><a href=""><i class="fa-brands fa-facebook-f"></i></a></li>
                            <li><a href=""><i class="fa-brands fa-twitter"></i></a></li>
                            <li><a href=""><i class="fa-brands fa-instagram"></i></a></li>
                            <li><a href=""><i class="fa-brands fa-youtube"></i></a></li>
                            <li><a href=""><i class="fa-brands fa-linkedin-in"></i></a></li>
                            <li><a href=""><i class="fa-brands fa-tiktok"></i></a></li>
                        </ul>
                    </div>
                </div>

                <!-- SERVICES -->
                <div class="services">
                    <h4>Services</h4>
                    <ul v-for="link in footerData.services">
                        <li><a href="">{{ link }}</a></li>
                    </ul>
                </div>

                <!-- RESOURCES -->
                <div class="resources">
                    <h4>Resources</h4>
                    <ul v-for="link in footerData.resources">
                        <li><a href="">{{ link }}</a></li>
                    </ul>
                </div>

                <!-- COMPANY -->
                <div class="company">
                    <h4>Company</h4>
                    <ul v-for="link in footerData.company">
                        <li><a href="">{{ link }}</a></li>
                    </ul>
                </div>
            </div>
        </div>
        <div class="footer-bottom">
            <div class="credits">
                <ul v-for="link in footerData.credits">
                    <li>{{ link }}</li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
p,
h4 {
    margin-left: 1rem;
}

p {
    font-size: 1.4rem;
}

a {
    color: black;

    &:hover {
        color: black;
        border-bottom: 2px solid black;
    }
}

.container {
    height: 600px;

    .footer-top {
        height: 400px;
        padding-top: 7rem;

        .row {
            display: flex;
            justify-content: space-between;

            .col {
                width: 300px;

                .socials ul {
                    display: flex;

                }
            }
        }
    }

    .footer-bottom {

        .credits {
            height: 200px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
    }
}
</style>