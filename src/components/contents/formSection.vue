<script>
export default {
    name: 'formSection'
}
</script>

<template>
    <div class="form-box">
        <div class="profile">
            <div class="profile-pic">
                <img src="" alt="">
            </div>
        </div>
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
</style>