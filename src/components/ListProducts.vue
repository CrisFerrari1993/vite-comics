<script>
export default {
    name: 'ListProducts',
    data() {
        return {
            cards: [
                {
                    text: 'DIGITAL COMICS',
                    img: 'public/img/card/buy-comics-digital-comics.png',
                    url: '#',
                    current: true,
                },
                {
                    text: 'DC MERCHANDISE',
                    img: 'public/img/card/buy-comics-merchandise.png',
                    url: '#',
                    current: false,
                },
                {
                    text: 'SUBSCRIPTION',
                    img: 'public/img/card/buy-comics-shop-locator.png',
                    url: '#',
                    current: false,
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    img: 'public/img/card/buy-comics-subscriptions.png',
                    url: '#',
                    current: false,
                },
                {
                    text: 'DC POWER VISA',
                    img: 'public/img/card/buy-dc-power-visa.svg',
                    url: '#',
                    current: false,
                }
            ]
        }
    }
}
</script>

<template>
    <section id="jumbotron">
        <img class="fill" src="../../public/img/jumbotron.jpg" alt="">
    </section>
    <main>
        <div class="container">
            <!-- __> Content goes here &lt;__ -->
            <div class="btn">
                <h3>CURRENT SERIES</h3>
            </div>
            <div class="row">
                <div class="col">
                    Prova
                </div>
            </div>
        </div>
    </main>
    <section>
        <div class="container">
            <ul>
                <li v-for="card in cards">
                    <a :href="card.url">
                        <img :src="card.img" alt="">
                        <span>{{ card.text }}</span>
                    </a>
                </li>
            </ul>
        </div>
    </section>
</template>

<style lang="scss" scoped>
// SCSS ONLY COMPONENT
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

h1,
h2,
h3,
h4,
h5,
h6 {
    color: $light;
}

main {
    background-color: #1c1c1c;
    padding: 2rem 0;

    .btn {
        background-color: #0282f9;
        width: fit-content;
        padding: 1rem 0.5rem;
        position: relative;
        bottom: 4rem;
    }
}

section {
    background-color: #0282f9;

    &#jumbotron {
        background-color: #1c1c1c;


        img {
            width: 100%;
            height: 500px;

            &.fill {
                object-fit: cover;
                object-position: top;
            }
        }
    }


    ul {

        list-style: none;
        @include center();
        display: flex;
        width: 100%;

        li {
            width: calc(100% / 5);
            height: fit-content;

        }

        li a {
            padding: 1rem;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-wrap: nowrap;
            text-decoration: none;
            font-weight: 600;
            color: $light;
            @include center();

            img {
                max-width: 30%;
                margin-right: 10px;
            }
        }
    }
}
</style>