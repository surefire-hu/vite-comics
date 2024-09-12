<script>
    export default {
    };
</script>

<template>
    <button class="sign-button">
        Sign-up now!
    </button>
</template>

<style scoped lang="scss">
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixin' as *;
    .sign-button{
        padding: 10px 10px;
        border: 2px solid $bg-primary;
        color: $color-white;
        background-color: transparent;
        cursor: pointer;
        @include uppercase;
    }
</style>