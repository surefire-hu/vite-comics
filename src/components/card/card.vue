<script>
export default {
    props: ['image', 'title']
};
</script>

<template>
    <li class="card">
        <img 
        :src="image" 
        :alt="title">
        <h4>{{ title }}</h4>
    </li>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/mixin' as *;

.card {
    img {
        width: 100%;
        display: block;
        height: 200px;
        object-fit: cover;
        margin-bottom: 10px;
    }
    h4 {
        @include uppercase;
        text-align: start;
    }
}
</style>