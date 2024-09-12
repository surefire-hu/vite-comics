<script>
import signBtn from '../general/signBtn.vue';
import AppFooterSocial from './AppFooterSocial.vue';

export default {
    name: 'AppFooterBottom',
    components: {
        signBtn,
        AppFooterSocial,
    }
};
</script>

<template> 
        <div id="footer-bottom">
            <div class="container">
                <signBtn></signBtn>
                <AppFooterSocial></AppFooterSocial>
            </div>
        </div>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/mixin.scss' as *;
@use '../../styles/partials/variables' as *;

    #footer-bottom {
        background-color: $bg-bottom-footer ;
        .container {
            padding: 20px 0;
            @include flex;
            @include container-size;
            justify-content: space-between;
        }
    }
</style>