<script>
export default {
    name: 'ListProducts',
    data() {
        return {
            cards: [
                {
                    text: 'DIGITAL COMICS',
                    img: '../assets/img/card/buy-comics-digital-comics.png'
                },
                {
                    text: 'DC MERCHANDISE',
                    img: '../assets/img/card/buy-comics-digital-comics.png'
                },
                {
                    text: 'SUBSCRIPTION',
                    img: '../assets/img/card/buy-comics-digital-comics.png'
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    img: '../assets/img/card/buy-comics-digital-comics.png'
                },
                {
                    text: 'DC POWER VISA',
                    img: '../assets/img/card/buy-comics-digital-comics.png'
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
                <li>
                    <a href="">
                        <img :src="cards.img" alt="">
                        prova
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


        li a {
            display: inline-block;
            padding: 3.5rem 1rem;
            text-decoration: none;
            font-weight: 600;
            color: $light;


            &.active,
            &:hover {
                color: $grey;
            }
        }
    }
}
</style>