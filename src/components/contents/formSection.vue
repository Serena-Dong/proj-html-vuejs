<script>
import { generalData } from '../../data/data'
import btn from './button.vue'
export default {
    name: 'formSection',
    components: { btn },
    data() {
        return {
            generalData,
            text: 'Get a Callback'
        }
    }
}
</script>

<template>
    <div class="form-box">
        <div class="profile">
            <div id="profile-pic">
                <img src="../../assets/img/contacts/marketing-consultant-expert.jpg" alt="">
            </div>
            <p id="name">Richard Madsen</p>
            <p id="role">Marketing Consultat Expert</p>
            <p id="phone-number"><i class="fa-solid fa-phone"></i>{{ generalData.phoneNumber }}</p>
        </div>
        <form action="submit">
            <input placeholder="Your Name*" type="text">
            <input placeholder="Your Email*" type="text">
            <input placeholder="Your Phone Number*" type="text">
            <btn :text="text"></btn>
        </form>
        <span>By submitting my data I agree to be contacted</span>
    </div>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/_variables' as *;

.form-box {
    text-align: center;

    margin-top: 6rem;
    width: 400px;
    min-height: 520px;

    background-color: $white;
    border-radius: 10px;
    box-shadow: 5px 5px 100px $grey;
}

.profile {
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

form {
    display: flex;
    flex-direction: column;
}

form>* {
    margin: 0.5rem 1.5rem 0.5rem;
    padding: 1rem;

    border-radius: 1rem;
    border: 1px solid $grey;
}

span {
    color: $grey;
    font-size: 0.7rem;
}
</style>