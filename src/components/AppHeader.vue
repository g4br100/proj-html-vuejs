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
    </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

header {
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
                margin: 0 3%;




                a {
                    color: black;
                    font-weight: 600;
                    font-size: 12px;
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