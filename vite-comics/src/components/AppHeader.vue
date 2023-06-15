<template>
    <header>
        <nav class="container">
            <div id="brandLogo">
                <img src="../assets/img/dc-logo.png" alt="DC Comics brand logo">
            </div>

            <div id="navigation">
                <div class="element">
                    <p>
                        Characters
                    </p>
                </div>

                <div class="element">
                    <p>
                        Comics
                    </p>
                </div>

                <div class="element">
                    <p>
                        Movies
                    </p>
                </div>

                <div class="element">
                    <p>
                        TV
                    </p>
                </div>

                <div class="element">
                    <p>
                    Games
                    </p>
                </div>

                <div class="element">
                    <p>
                        Collectibles
                    </p>
                </div>

                <div class="element">
                    <p>
                        Videos
                    </p>
                </div>

                <div class="element">
                    <p>
                        Fans
                    </p>
                </div>

                <div class="element">
                    <p>
                        News
                    </p>
                </div>

                <div class="element">
                    <p>
                        Shop
                    </p>
                </div>
            </div>
        </nav>
    </header>
</template>

<script>
export default {
    name: "AppHeader",
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