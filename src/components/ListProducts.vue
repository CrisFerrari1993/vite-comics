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
    <main>
        <div class="container">
            <h1>
                __> Content goes here &lt;__
            </h1>
        </div>
    </main>
    <section>
        <div class="container">
            <ul>
                <li v-for="card in cards">
                    <a :href="card.url">
                        <div class="img-container">
                            <img :src="card.img" alt="">
                        </div>
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

main {
    background-color: #1c1c1c;
    padding: 2rem 0;
}

section {
    background-color: #0282f9;
    padding: 2rem 0;

    ul {
        list-style: none;
        @include center();
        padding: 1rem 0;


        li a {
            margin: 2rem 3rem;
            display: flex;
            align-items: center;
            flex-wrap: nowrap;
            text-decoration: none;
            font-weight: 600;
            color: $light;

            img {
                max-width: 100%;
            }

            &.active,
            &:hover {
                color: $grey;
            }


        }
    }
}
</style>