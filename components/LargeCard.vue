<template>
    <div class="col-md-4 col-sm-12 card">
        <div class="card-body">
            <img class="image w-100" :src="require(`@/assets/images/${card.image || 'fe1.jpg'}`)" alt="">
        <h3 class="header">{{ card.title }}</h3>
        <p class="snippet">
            {{card.snippet }}
        </p>
        </div>
    </div>
</template>

<script>
    export default {
        props: ['card'],
    }
</script>

<style scoped>
    .card {
        border: none;
        overflow: hidden;
        padding: 0;
        cursor: pointer;
    }
    .image {
        border-radius: 0.5rem;
        height: 12rem;
    }
    .header {
        font-size: 1.15rem;
        margin-top: 0.4rem;
    }
    .snippet {
        color: grey
    }
</style>