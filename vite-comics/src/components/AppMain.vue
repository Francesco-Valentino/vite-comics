<template>
    <main>
        <div>
            <div class="jumbotron">
                <img src="../assets/img/jumbotron.jpg" alt="DC Comics Jumbotron">
            </div>

            <section id="upperMain">
                <ComicsList/>
            </section>

            <section id="actionsBar">

            </section>
        </div>
    </main>
</template>

<script>
import ComicsList from './ComicsList.vue';

export default {
    name: "AppMain",

    components: {
        ComicsList,
    },
}
</script>

<style lang="scss" scoped>
    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;
    section#upperMain{
        background-color: #1C1C1C;
        display: flex;
        align-items: center;

        h1{
        color: white;
        }
    }

    div.jumbotron{
            height: 250px;

            img{
                height: 100%;
                width: 100%;
                object-fit: cover;
                object-position: top;
            }
        }

    section#actionsBar{
        height: 140px;
        background-color: $themeColor;
    }
    
</style>