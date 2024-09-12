<script>
import logo from '../general/logo.vue';
import AppNavList from './AppNavList.vue';
import AppJumbo from './AppJumbo.vue';

export default {
    components: {
        logo,
        AppNavList,
        AppJumbo,
    }
};
</script>

<template>
    <header>
        <div id="dc-navbar">
            <logo></logo>
            <AppNavList></AppNavList>
        </div>
        <AppJumbo></AppJumbo>
    </header>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixin' as *;

    #dc-navbar {
        @include container-size;
        @include flex;
        justify-content: space-between;
        height: $size-header;
    } 

</style>