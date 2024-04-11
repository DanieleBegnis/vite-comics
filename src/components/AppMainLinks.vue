<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            links: [
                {
                    text: 'DIGITAL COMICS',
                    photo: ''
                },
                {
                    text: 'DC MERCHANDISE',
                    active: true
                },
                {
                    text: 'SUBSCRIPTION',
                    active: false
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    active: false
                },
                {
                    text: 'DC POWER VISA',
                    active: false
                },
            ]
        }
    }
}
</script>

<template>
    <main class="d-flex">
        <div class="container d-flex ">
            <div class="row">
                <div class="col-12 d-flex align-items-center" >
                    <ul class="d-flex py-5">
                        <li v-for="link in links">
                            <a href="#">{{ link.text }}</a>
                            <img :src="./.......{ link.photo}" alt="">
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </main>
</template>

<style scoped lang="scss">
    @use '../style/partials/variables' as *;
    main {
        background-color: $brand-primary;
    }
    ul {
        a {
            color: #fff;
        }
    }
</style>