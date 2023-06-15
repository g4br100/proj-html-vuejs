<script>
export default {
    name: "AppFooter",
    data() {
        return {
            links: [
                {
                    text: "Shop",
                    url: "#",
                    current: false,
                },
                {
                    text: "About",
                    url: "#",
                    current: false,
                },
                {
                    text: "Gallery",
                    url: "#",
                    current: false,
                },
                {
                    text: "Locations",
                    url: "#",
                    current: false,
                },
                {
                    text: "Journal",
                    url: "#",
                    current: false,
                },
                {
                    text: "Orders",
                    url: "#",
                    current: false,
                },
            ]
        }
    }
}
</script>

<template>
    <section>
        <div class="container">
            <div class="news">
                <a href="/" class="brand">
                    <img src="../assets/images/avada-bakery-logo.png" alt="backery">
                </a>
                <ul>
                    <li v-for="link in links">
                        <a :href="link.url" :class="{ active: link.current }">{{ link.text }}</a>
                    </li>
                </ul>
            </div>
            <div class="news">
                <h3 class="my-heading">Subscribe to our Newsletter</h3>
                <div class="sender">
                    <input type="email" placeholder="Enter email address*">
                    <button>Subscribe</button>
                </div>
                <div>
                    <i class="'fa-brands fa-instagram'"></i>
                </div>
            </div>
        </div>
    </section>
    <section>
        <div class="container">
            <small id="copy">© Copyright 2012-2020 | Avada Theme by ThemeFusion | All Rights Reserved |
                Powered by Wordpress</small>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;


.brand {
    padding: 20px 0;
}

#copy {
    padding: 50px 0;
}

.container {
    @include my-display-flex-1;
    margin: 0 50px;

    ul {
        @include center ();
        justify-content: start;

        li {
            margin: 0 2%;

            a {
                color: $secondary-color;
                font-weight: 600;
                font-size: 12px;

            }

        }
    }

}

.news {
    display: flex;
    flex-direction: column;
    width: 45%;
}




.my-heading {
    margin-top: 0;
    margin-bottom: 0.5em;
    font-size: 1.5em;
    text-align: right;
}



.sender {
    display: flex;
    justify-content: end;
    margin: 50px;

    input {
        background-color: white;
        border: 1px solid;
        padding: 0.5em 0.75em;
        width: 50%;
    }
}

button {
    color: white;
    background-color: $secondary-color;
    padding: 0.5em 1em;
    border-radius: 6px;
    margin-left: 20px;
}
</style>