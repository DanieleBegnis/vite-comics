<script>
export default {
    name: 'AppFooterFinal',
    data() {
        return {
            links: [
                {
                    photo: 'buy-comics-digital-comics.png'
                },
                {
                    photo: 'buy-comics-merchandise.png'
                },
                {
                    photo: 'buy-comics-subscriptions.png'
                },
                {
                    photo: 'buy-comics-shop-locator.png'
                },
                {
                    photo: 'buy-dc-power-visa.svg'
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
                <div class="col-6 d-flex align-items-center">
                    <div class="subtitle font-weight-bold fs-5"> FOLLOW US</div>
                    <ul></ul>
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