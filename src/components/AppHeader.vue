<script>
import { headerData } from '../data/data';
import { generalData } from '../data/data';

export default {
    name: 'AppHeader',
    data() {
        return {
            headerData,
            generalData
        }
    },
    computed: {
        logoSrc() {
            const url = new URL(headerData.logo, import.meta.url);
            return url.href
        }
    }
}
</script>

<template>
    <header>
        <div class="container">

            <!-- LOGO -->
            <div class="logo">
                <img :src=logoSrc alt="">
            </div>

            <!-- NAV -->
            <div class="nav">
                <ul v-for="link in headerData.navbar">
                    <li><a href="">{{ link }}</a></li>
                </ul>

            </div>

            <!-- CONTACTS -->
            <div class="contacts">
                <!-- PHONE NUMBER -->
                <a href=""><i class="fa-solid fa-phone"></i>{{ generalData.phoneNumber }}</a>

                <!-- BUTTON -->
                <button class="transparent"><a href="">Free Quote</a></button>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/_variables' as *;

.container {
    height: 100px;

    display: flex;
    justify-content: space-between;
    align-items: center;
}

.nav {
    display: flex;
    align-items: center;
}

.contacts>* {
    margin-left: 2rem;
}

a {
    color: black;

    &:hover {
        color: $white;

        padding: 2.5rem 0 2.5rem;
        border-bottom: 2px solid $ochre;
    }
}

button a {
    color: $ochre;
}
</style>
