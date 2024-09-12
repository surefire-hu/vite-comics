<script>
import AppFooterList from './AppFooterList.vue';
import AppFooterBottom from './AppFooterBottom.vue';

export default {
    components: {
        AppFooterList,
        AppFooterBottom,
    }
};
</script>

<template>
    <footer id="dc-footer">
        <div id="footer-top">
            <div class="container">
                <AppFooterList></AppFooterList>  
            </div>
        </div>
        <AppFooterBottom></AppFooterBottom>
    </footer>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixin' as *;

#footer-top {
    background-image: url('/footer-bg.jpg');
    background-size: cover;
    .container{
        @include container-size;
        @include flex;
        justify-content: space-between;
        overflow: hidden;
    }
}
</style>