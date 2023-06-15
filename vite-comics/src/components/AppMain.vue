<template>
    <main>
        <div>
            <section id="upperMain">
                <h1 class="container">
                    ---Content goes here---
                </h1>
            </section>

            <section id="actionsBar">

            </section>
        </div>
    </main>
</template>

<script>
export default {
    name: "AppMain",
}
</script>

<style lang="scss" scoped>
    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;
    section#upperMain{
        height: 100px;
        background-color: #1C1C1C;
        display: flex;
        align-items: center;

        h1{
        color: white;
        }
    }

    section#actionsBar{
        height: 140px;
        background-color: $themeColor;
    }
    
</style>