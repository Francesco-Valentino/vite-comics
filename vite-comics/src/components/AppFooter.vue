<template>
    <footer>
        <section id="upperFooter">

            <div class="container colWrap">
                <div class="column">
                    <article class="footerArticle">
                        <h5>
                            DC Comics
                        </h5>

                        <p v-for="dcComicsEl in dcComicsFooterEl">
                            {{ dcComicsEl }}
                        </p>
                    </article>

                    <article class="footerArticle">
                        <h5>
                            Shop
                        </h5>

                        <p v-for="shopEl in shopFooterEl">
                            {{ shopEl }}
                        </p>
                    </article>
                </div>

                <div class="column">
                    <article class="footerArticle">
                        <h5>
                            DC
                        </h5>

                        <p v-for="dcEl in dcFooterEl">
                            {{ dcEl }}
                        </p>
                    </article>
                </div>

                <div class="column">
                    <article class="footerArticle">
                        <h5>
                            Sites
                        </h5>

                        <p v-for="sitesEl in sitesFooterEl">
                            {{ sitesEl }}
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

    data(){
        return{
            dcComicsFooterEl: [
                "Characters",
                "Comics",
                "Movies",
                "TV",
                "Games",
                "Videos",
                "News"
            ],

            shopFooterEl: [
                "Shop DC",
                "Shop DC Collectibles"
            ],

            dcFooterEl: [
                "Terms Of Use",
                "Privacy policy (new)",
                "Ad Choices",
                "Advertising",
                "Jobs",
                "Subscriptions",
                "Talent Workshops",
                "CPSC Certificates",
                "Ratings",
                "Shop Help",
                "Contact Us"
            ],

            sitesFooterEl: [
                "DC",
                "MAD Magazine",
                "DC Kids",
                "DC Universe",
                "DC Power Visa"
            ]
        }
    },
}
</script>

<style lang="scss">
    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;

    div.colWrap{
        display: flex;
        margin-left: 10rem;

        div.column{
            margin: 2rem 1rem 0 1rem;

            article.footerArticle{
                margin-bottom: 1.4rem;
            }
        }
    }

    section#upperFooter{
        background-image: url('../assets/img/footer-bg.jpg');
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