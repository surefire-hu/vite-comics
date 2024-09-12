<script>
export default {
}
</script>

<template>
    <div class="bottom-right">
        <h3>Follow Us</h3>
        <div class="social-links">
            <a href="" target="">
                <img class="img-logo" src="/footer-facebook.png" alt="">
            </a>
            <a href="" target="">
                <img class="img-logo" src="/footer-twitter.png" alt="">
            </a>
            <a href="" target="">
                <img class="img-logo" src="/footer-youtube.png" alt="">
            </a>
            <a href="" target="">
                <img class="img-logo" src="/footer-pinterest.png" alt="">
            </a>
            <a href="" target="">
                <img class="img-logo" src="/footer-periscope.png" alt="">
            </a>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixin' as *;
.bottom-right {
    @include flex;
    gap: 20px;
    color: $bg-primary;
    .social-links {
        display: flex;
        gap: 15px;
        cursor: pointer;
        .img-logo {
            width: 35px;
            display: block;
            padding: 5px;
        }
    }
}

</style>