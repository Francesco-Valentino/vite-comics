<template>
    <footer>
        <section id="upperFooter">

            <div class="container">
                <div class="column">
                    <article class="footerArticle">
                        <h5>
                            Lorem
                        </h5>

                        <p>
                            Ipsum
                        </p>

                        <p>
                            Ipsum
                        </p>

                        <p>
                            Ipsum
                        </p>

                        <p>
                            Ipsum
                        </p>
                    </article>
                </div>
            </div>
            
        </section>

        <section id="bottomFooter">

        </section>
    </footer>
</template>

<script>
export default {
    name: "AppFooter",
}
</script>

<style lang="scss">
    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;

    section#upperFooter{
        background-image: url("../assets/img/footer-bg.jpg");
        background-repeat: no-repeat;
        background-size: cover;
        height: 300px;

        h5{
            text-transform: uppercase;
            color: white;
            margin-bottom: .7rem;
        }

        p{
            font-size: .7rem;
            color: grey;
            margin-bottom: .3rem;
        }
    }

    section#bottomFooter{
        height: 100px;
        background-color: #303030;
    }
</style>