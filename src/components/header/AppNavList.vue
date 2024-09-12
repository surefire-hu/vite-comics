<script>
export default {
    data() {
        return {
            menu: [
                {   
                    nome: 'Characters',
                    href: '#',
                    active: false,
                },
                {
                    nome: 'Comics',
                    href: '#',
                    active: true,
                },
                {
                    nome: 'Movies',
                    href: '#',
                    active: false,
                },
                {
                    nome: 'Tv',
                    href: '#',
                    active: false,
                },
                {
                    nome: 'Games',
                    href: '#',
                    active: false,
                },
                {
                    nome: 'Collectibles',
                    href: '#',
                    active: false,
                },
                {
                    nome: 'Videos',
                    href: '#',
                    active: false,
                },
                {
                    nome: 'Fans',
                    href: '#',
                    active: false,
                },
                {
                    nome: 'News',
                    href: '#',
                    active: false,
                },
                {
                    nome: 'Shop',
                    href: '#',
                    active: false,
                }
            ]
        }
    },
};
    
</script>

<template>

    <ul class="list-links">
        <li class="link" v-for="li in menu">
            <a :href="li.href" :class="{'active': li.active}">{{ li.nome }}</a>
        </li>
    </ul>
</template>

<style scoped lang="scss">
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixin' as *;
.list-links {
    display:flex;
    gap: 35px;
    @include uppercase;
    .link {
        list-style-type: none;
        line-height: $size-header;
        border-bottom: 2px solid transparent;

        
        

        a {
        &.active {
            color: $bg-primary;
            border-bottom: 2px solid $bg-primary;
        }
        &:hover {
            color: $bg-primary;
            border-bottom: 2px solid $bg-primary;
        }
            all: unset;
            font-weight: 600;
            text-decoration: none;
        }
    }
}
</style>