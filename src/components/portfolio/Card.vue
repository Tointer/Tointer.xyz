<template>
    <g-link :to="`/games/${card.to}`">
        <div class="card shadow border-0 my-4">
            <img class="card-img-top" :src="card.img" alt="Card image cap">
            <div class="card-body">
                <blockquote class="blockquote mb-0">
                    <p>{{ card.text }}</p>
                    <footer class="blockquote-footer"><cite title="Source Title">Tointer Games</cite></footer>
                </blockquote>
            </div>
        </div>
    </g-link>
</template>

<script>
    export default {
        name: "Card",
        props: {
            card: Object,
        },
    }
</script>

<style scoped>

</style>