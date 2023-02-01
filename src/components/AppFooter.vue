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
                    <h3>Grow Your Online Business Strategically, and Improve Customer Retention</h3>
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
                    <ul v-for="link in footerData.services">
                        <li><a href="">{{ link }}</a></li>
                    </ul>
                </div>

                <!-- COMPANY -->
                <div class="company">
                    <h4>Company</h4>
                    <ul v-for="link in footerData.services">
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
h3,
h4 {
    margin-left: 1rem;
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
    border: 2px solid black;

    .footer-top {
        height: 400px;
        border: 2px solid black;

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
        border: 2px solid black;

        .credits {
            height: 200px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
    }
}
</style>