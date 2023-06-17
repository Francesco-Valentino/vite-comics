<template>
    <header>
        <nav class="container">
            <div id="brandLogo">
                <img src="../assets/img/dc-logo.png" alt="DC Comics brand logo">
            </div>

            <div id="navigation">
                <div v-for="element in navElements" class="element">
                    <p>
                        {{ element }}
                    </p>
                </div>            
            </div>
        </nav>
    </header>
</template>

<script>
export default {
    name: "AppHeader",

    data(){
        return{
            navElements: [
            "Characters",
            "Comics",
            "Movies",
            "TV",
            "Games",
            "Collectibles",
            "Videos",
            "Fans",
            "News",
            "Shop"
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;

    nav.container{
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: .7rem;

        div#brandLogo img{
            width: 70px;
        }

        div#navigation{
            display: flex;
            justify-content: space-between;
            flex-wrap: nowrap;
            text-transform: uppercase;

            p{
                font-size: .6rem;
                padding: 0 .7rem;
            }
        }
    }
</style>