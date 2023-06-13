<script>
export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    text: "HOME",
                    url: "#",
                    current: false,
                },
                {
                    text: "SHOP",
                    url: "#",
                    current: true,
                },
                {
                    text: "ABOUT",
                    url: "#",
                    current: false,
                },
                {
                    text: "GALLERY",
                    url: "#",
                    current: false,
                },
                {
                    text: "LOCATIONS",
                    url: "#",
                    current: false,
                },
                {
                    text: "JOURNAL",
                    url: "#",
                    current: false,
                },
                {
                    text: "CONTACT",
                    url: "#",
                    current: false,
                },
                {
                    text: "MY ACCOUNT",
                    url: "#",
                    current: false,
                }
            ]
        }
    }
}
</script>

<template>
    <header>
        <div>
            <div class="logo">
                <a href="/" class="brand">
                    <img src="../assets/images/avada-bakery-logo.png" alt="backery">
                </a>
            </div>
            <nav>
                <ul>
                    <li v-for="link in links">
                        <a :href="link.url" :class="{ active: link.current }">{{ link.text }}</a>
                    </li>
                </ul>
            </nav>
        </div>
        <div class="perfect-bread-text-container">
            <h4>fresh & tasty bakery every day</h4>
            <h1>The Perfect Fresh Bread</h1>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Incidunt ducimus sint distinctio voluptatem quod.
                Modi voluptatem impedit inventore dolorem odit?</p>

            <button class="explore">
                <a href="#">Explore our products</a>
            </button>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

header {
    padding: 0 2%;
    height: 100vh;
    background-image: url(../assets/images/hero-header-bakery.jpg);
    background-size: cover;
}

.perfect-bread-text-container {
    padding-top: 100px;
    width: 30vw;
    height: 30vh;
    margin-left: 150px;

    h4 {
        color: $secondary-color;
        font-size: 11px;
        text-transform: uppercase;
        font-weight: 100;
    }

    h1 {
        color: $secondary-color;
        font-size: 50px;
        line-height: 60px;
        margin: 30px 0;
    }

    p {
        color: black;
        font-size: 1.2rem;
        line-height: 30px;

    }

    button {
        margin: 40px 0;
    }
}

header :first-child {
    @include my-display-flex-1 ();
    align-items: center;

    .logo {

        @include center ();

        img {
            width: 178px;

        }
    }

    nav {
        width: 50%;

        ul {
            margin: 0;
            @include center ();

            li {
                margin: 0 2%;

                a {
                    color: $secondary-color;
                    font-weight: 600;
                    font-size: 12px;
                    text-transform: uppercase;

                }

                &:active,
                &:hover {
                    color: $primary-color;
                    border-bottom: 5px solid $primary-color;
                }


            }
        }
    }
}
</style>