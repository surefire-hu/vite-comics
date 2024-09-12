<script>
import cardsList from '../card/cardList.vue';

export default {
    components: {
        cardsList,
    }
};
</script>

<template>
    <section id="dc-main-top">
        <div class="container">
            <h2 class="label-section">Current series</h2>
            <cardsList></cardsList>
        </div>
    </section> 
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixin.scss' as *;

#dc-main-top {            
    background-color: $bg-main;
    .container {
        @include container-size;
        position: relative;
        .label-section {
            background-color: $bg-primary;
            color: $color-white;
            padding: 10px 20px;
            display: inline-block;
            position: absolute;
            top: -25px;
            @include uppercase;
        }
    }
}
</style>