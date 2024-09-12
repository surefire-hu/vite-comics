<script>
export default {
    data () {
        return {
            Icons: [
                {
                    nome: 'Digital comics',
                    src: '/buy-comics-digital-comics.png',
                    alt: 'digital-comics-image'
                },
                {
                    nome: 'Dc merchandise',
                    src: '/buy-comics-merchandise.png',
                    alt: 'comics-merchandise'
                },
                {
                    nome: 'Subscription',
                    src: '/buy-comics-subscriptions.png',
                    alt: 'comics-subscriptions'
                },
                {
                    nome: 'Comics shop locator',
                    src: '/buy-comics-shop-locator.png',
                    alt: 'shop-locator'
                },
                {
                    nome: 'Dc power visa',
                    src: '/buy-dc-power-visa.svg',
                    alt: 'power-visa'
                },
            ]
        }
    }
}
</script>

<template>
    <div id="dc-main-bottom">
        <div class="container">
            <ul class="list-icons">
                <li class="icon-content" v-for="li in Icons">
                    <img :src="li.src" :alt="li.alt">
                    <h3>{{ li.nome }}</h3>
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixin' as *;

#dc-main-bottom {            
    background-color: $bg-primary;
    color: $color-white;

    .container {
        @include container-size;
        padding: 50px 0;

        .list-icons {
            @include flex;
            justify-content: center;
            gap: 30px;

            .icon-content {
                @include flex;
                @include uppercase;
                justify-content: center;
                gap: 15px;

                img {
                    width: 50px;
                }
            }
        }
    }
}
</style>