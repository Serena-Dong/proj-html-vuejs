<script>
import { generalData } from '../../data/data';
export default {
    name: 'contact card',
    data() {
        return {
            generalData
        }
    }
}
</script>

<template>
    <section>
        <div class="container">
            <div class="profile">
                <div id="profile-pic">
                    <img src="../../assets/img/contacts/marketing-expert-cta.png" alt="">
                </div>
                <div id="profile-details">
                    <p id="name">Sandy Reiff</p>
                    <p id="role">Marketing Consultat Expert</p>
                </div>

            </div>
            <div class="detail">
                <p>Drive Leads and Sales with Avada</p>
            </div>
            <button class="transparent"><a href=""><i class="fa-solid fa-phone"></i>{{
                generalData.phoneNumber
            }}</a></button>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables' as *;

.container {
    height: 100px;
    box-shadow: 5px 5px 10px rgba(0, 0, 0, 0.288);
    border-radius: 1rem;

    display: flex;
    align-items: center;
    justify-content: space-around;

    .profile {
        display: flex;
        align-items: center;

        #profile-pic img {
            height: 60px;
            border-radius: 5rem;
        }

        #profile-details {

            margin-left: 1rem;

            #name {
                font-size: 1.2rem;
                margin-bottom: 0.2rem;
            }

            #role {
                color: $grey;
                font-size: 0.8rem;

            }
        }

    }

    .detail p {
        font-size: 1.5rem;
    }
}
</style>