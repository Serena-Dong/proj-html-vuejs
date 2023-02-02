<script>
import { generalData } from '../../data/data'
export default {
    name: 'formSection',
    data() {
        return {
            generalData
        }
    }
}
</script>

<template>
    <div class="form-box">
        <div class="profile">
            <div id="profile-pic">
                <img src="../../assets/img/marketing-consultant-expert.jpg" alt="">
            </div>
            <p id="name">Richard Madsen</p>
            <p id="role">Marketing Consultat Expert</p>
            <p id="phone-number"><i class="fa-solid fa-phone"></i>{{ generalData.phoneNumber }}</p>
        </div>
        .
    </div>
</template>

<style lang="scss" scoped>
@use '../../assets/css/scss/partials/_variables' as *;

.form-box {
    margin-top: 8rem;
    width: 400px;
    height: 470px;

    background-color: $white;
    border-radius: 10px;
    box-shadow: 5px 5px 100px $grey;
}

.profile {
    text-align: center;

    #profile-pic img {
        height: 70px;
        border-radius: 5rem;
    }

    #name {
        font-size: 1.5rem;
    }

    #role {
        color: $grey;
    }

    #phone-number {
        color: $ochre;
        margin-right: 1rem;
    }
}

.profile>* {
    margin: 1rem;
}
</style>