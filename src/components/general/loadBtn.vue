<script>
export default {
}
</script>

<template>
    <button class="load-button">
        <h4>Load more</h4>
    </button>

</template>

<style lang="scss" scoped>

@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixin' as *;

.load-button {
    all: unset;
    background-color: $bg-primary;
    padding: 10px 50px;
    color: $color-white;
    @include uppercase;
    cursor: pointer;
}
</style>