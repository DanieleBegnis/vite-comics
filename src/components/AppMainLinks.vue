<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            links: [
                {
                    text: 'DIGITAL COMICS',
                    photo: 'buy-comics-digital-comics.png'
                },
                {
                    text: 'DC MERCHANDISE',
                    photo: 'buy-comics-merchandise.png'
                },
                {
                    text: 'SUBSCRIPTION',
                    photo: 'buy-comics-subscriptions.png'
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    photo: 'buy-comics-shop-locator.png'
                },
                {
                    text: 'DC POWER VISA',
                    photo: 'buy-dc-power-visa.svg'
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
                        <li class="px-3 d-flex align-items-center fs-6" v-for="link in links">
                            <img class="mx-3" :src="'src/assets/img/' + link.photo" alt="">
                            <a class="px-6" href="#">{{ link.text }}</a>
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
        img {
            max-width: 50px;
        }
    }
</style>