<script>
</script>

<template>
    <footer>
        <div class="container">
            <div class="row justify-content-between">
                <div class="col-6">
                    <button type="button" class="btn my-3">SIGN-UP! NOW</button>
                </div>
                <div class="col-6"></div>
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
    }
</style>