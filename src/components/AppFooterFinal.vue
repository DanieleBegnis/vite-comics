<script>
export default {
    name: 'AppFooterFinal',
    data() {
        return {
            links: [
                {
                    photo: 'footer-facebook.png'
                },
                {
                    photo: 'footer-periscope.png'
                },
                {
                    photo: 'footer-pinterest.png'
                },
                {
                    photo: 'footer-twitter.png'
                },
                {
                    photo: 'footer-youtube.png'
                },
            ]
        }
    }
}
</script>

<template>
    <footer>
        <div class="container">
            <div class="row justify-content-between">
                <div class="col-6">
                    <button type="button" class="btn my-3">SIGN-UP! NOW</button>
                </div>
                <div class="col-6 d-flex align-items-center justify-content-end">
                    <div class="subtitle font-weight-bold fs-5"> FOLLOW US</div>
                    <ul class="d-flex">
                        <li class=" d-flex align-items-center " v-for="link in links">
                            <img class="mx-3" :src="'src/assets/img/' + link.photo" alt="">
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;
    footer {
        background-color: $brand-secondary;
        .btn {
            color: #fff;
            border: 3px solid $brand-primary;
            border-radius: 0
        }
        .subtitle {
            color: $brand-primary;
        }
    }
</style>