<script>
    export default {
        data () {
            return {
                menu: [
                {
                    nomeClasse: 'Dc comics',
                    links: ['Characters', 'Comics', 'Movies', 'TV', 'Games', 'Videos', 'News'],
                },
                {
                    nomeClasse: 'Shop',
                    links: ['Shop Dc', 'Shop Dc Collectibles'],
                },
                {
                    nomeClasse: 'Dc',
                    links: ['Terms Of Use', 'Privacy policy (New)', 'Ad Choices', 'Advertising', 'Jobs', 'Subscriptions', 'Talent Workshops', 'CPSC Certificates', 'Ratings', 'Shop Help', 'Contact Us'],
                },
                {
                    nomeClasse: 'Sites',
                    links: ['Dc', 'Mad Magazine', 'Dc Kids', 'Dc Universe', 'Dc Power Visa'],
                }],
            }
        },
    };
</script>

<template>
    <ul class="menu-footer-nav"> 
        <li v-for="classelink in menu" class="sections">
            <h2>{{ classelink.nomeClasse }}</h2>
            <ul class="labels">
                <li class="label-link" v-for="link in classelink.links">
                    <a href="#">{{ link }}</a>
                </li>
            </ul>
        </li>
    </ul>
    <img class="logo-bg" src="/dc-logo-bg.png" alt="dc-logo-bg">
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixin' as *;
.menu-footer-nav {
    display: flex;
    flex-direction: column;
    color: $color-white;
    max-height: 400px;
    padding: 40px 0 60px;
    gap: 10px 40px;
    flex-wrap: wrap;
    flex-grow: 1;
    align-content: start; 
    .sections {
        @include uppercase;
    }
    .labels {
        display: flex;
        flex-direction: column;
        
        .label-link {
            font-size: 10px;
            color: rgb(171, 169, 169);
            padding-top: 8px;
            &:hover {
                color: $color-white;
                cursor: pointer;
            }
        }
    }
}
.logo-bg {
        width: 600px;
        max-height: 400px;
    object-fit: cover;
}
</style>