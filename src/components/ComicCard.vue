<script>
export default {
    name: 'ComicCard',
    props: ['cardInfo']
}
</script>

<template>
    <div class="comic-card">
        <div class="comic-image">
            <img :src="cardInfo.thumb">
        </div>

        <h3>{{ cardInfo.series }}</h3>
    </div>

</template>

<style>
@use '../style/partials/variables' as *;
    .comic-card {
        width: calc((100% / 6) - 12px);
        img {
            display: block;
            width: 100%;
            height: 190px;
            object-fit: cover;
        }
    }
</style>