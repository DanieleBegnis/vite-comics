<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            links: [
                {
                    text: 'Characters',
                    active: false
                },
                {
                    text: 'Comics',
                    active: true
                },
                {
                    text: 'Movies',
                    active: false
                },
                {
                    text: 'TV',
                    active: false
                },
                {
                    text: 'Games',
                    active: false
                },
                {
                    text: 'Collectibles',
                    active: false
                },
                {
                    text: 'Videos',
                    active: false
                },
                {
                    text: 'Fans',
                    active: false
                },
                {
                    text: 'News',
                    active: false
                },
                {
                    text: 'Shop',
                    active: false
                }
            ]
        }
    }
}
</script>

<template>
    <header class="d-flex">
        <div class="container d-flex ">
            <div class="row">
            <div class="col-6">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <div class="col-6 d-flex align-items-center" >
                <ul class="d-flex">
                <li :class="{'active': link.active}" v-for="link in links">
                    <a href="#">{{ link.text }}</a>
                </li>
            </ul>
            </div>
        </div>
        </div>
    </header>
</template>

<style scoped lang="scss">
    @use '../style/partials/variables' as *;
    .col-6 {
        img {
            padding: 20px, 0;
        }
        ul {
            a {
                color: #000;
                &.active {
                color: $brand-primary;
            }
            }
        }
        li {
            padding: 12px;
            &.active {
                color: $brand-primary;
                border-bottom: 3px solid $brand-primary;
            }
        }
    }
</style>