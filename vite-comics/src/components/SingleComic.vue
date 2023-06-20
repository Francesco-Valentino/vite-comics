<template>
    <div class="singleComicCard">
        <img :src="thumbnail" :alt="name + ' thumbnail'">
    
        <h3>
            {{ name }}
        </h3>
    </div>
    
</template>

<script>
export default {
    name: "SingleComic",

    props: {
        thumbnail: String,
        name: String,
    },
}
</script>

<style lang="scss" scoped>
    div.singleComicCard{
        width: calc((100% / 6) - 1rem);
        margin: 1.5rem .5rem;
        text-align: center;
    }

    img{
        width: 100%;
    }
</style>