<script>
export default {
    name: "AppMain",
};
</script>

<template>
    <main class="site-main">
        <div class="cookie-container">
            <div class="cookie-text">
                <h6 class="title-min">our products</h6>
                <h1 class="title-medium">All our delectable pastries are backed fresh in our Kitchen very morning, and are
                    made with all-natural,
                    all
                    organic ingredients</h1>
                <button>Start Shopping</button>
            </div>
            <div class="cookie-image-container">
                <div class="cookie-image-1">
                    <img src="../assets/images/choco-chip-cookies-1200x1530.jpg" alt="">
                </div>
                <div class="cookie-image-2">
                    <img src="../assets/images//strawberry-jam-cookies-1200x1530.jpg" alt="">
                </div>
            </div>
        </div> <!--cookie container end-->
        <div class="moments-container">
            <div class="moments-title-container">
                <h6 class="title-min">corporate & weddings</h6>
                <h1 class="title-medium">Baking Special Moments</h1>
            </div>
            <div class="moments-image-container">
                <div class="moments-image-1">
                    <img src="../assets/images/corporate-bg.jpg" alt="">
                </div>
                <div class="moments-image-1">
                    <img src="../assets/images/wedding-bg.jpg" alt="">
                </div>
            </div>
        </div> <!--moments container end-->
        <div class="product-container">
            <div class="product-text">
                <h1 class="title-medium">Find a freshly baked product perfect for you</h1>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Iste ipsam cumque doloremque, perspiciatis
                    error aut
                    nemo harum sapiente voluptas fugiat!</p>
                <button>Shop All Products</button>
            </div>
            <div class="product-image-container"> <!--CAROUSEL-->
                <img src="../assets/images/choco-chip-cookies-1200x1530.jpg" alt="">
                <img src="../assets/images/strawberry-jam-cookies-1200x1530.jpg" alt="">
                <img src="../assets/images/strawberry-donut-1200x1530.jpg" alt="">
                <img src="../assets/images/perfect-macarons-1200x1530.jpg" alt="">
            </div>
        </div> <!--product container end-->
        <div class="tell-us-container">
            <div>
                <h1>Tell us what you have in mind</h1>
                <h2>01</h2>
            </div>
            <div class="tell-us-text">
                <h3>manual ingredient selection</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Rerum numquam fugit accusamus eum mollitia
                    suscipit
                    nisi incidunt ad! Aut, nihil sit quibusdam ad doloremque dolores esse provident porro perspiciatis unde
                    excepturi veniam fuga repudiandae iusto vel, tempora alias laboriosam voluptatibus.</p>
            </div>
        </div> <!--tell us container end-->
        <div class="we-start-container">
            <div class="we-start-image">
                <div>
                    <h1>We Start Baking</h1>
                    <h2>02</h2>
                </div>
                <div class="we-start-image-text">
                    <h3>sweet & delicious</h3>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. At, vero suscipit. Mollitia animi optio eos
                        delectus
                        pariatur dicta, consectetur, totam, doloribus tempore assumenda soluta provident rem debitis culpa
                        repellendus
                        velit?</p>
                </div>
            </div>
            <div class="we-start-text">
                <div>
                    <h3 class="title-min">dont just take our word for it</h3>
                    <h5>"Finally found an alternative to the mass produced products.Something that incorporates real organic
                        ingredients, nutrient dense wellness while promoting sustainability and activity."</h5>
                    <h6>Rachel Cooper, Founder</h6>
                </div>
            </div>
        </div> <!--we start container end-->
        <div class="delivered-container">
            <div class="delivered-title">
                <h1>Delivered to your home</h1>
                <h2>03</h2>
            </div>
            <div class="delivered-text">
                <h3>baked to order & gift wrapped</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Facilis dolore et culpa! Laudantium
                    perspiciatis,
                    libero sit quaerat molestias mollitia inventore dignissimos ipsum velit numquam consectetur expedita
                    minus
                    dolorem vel error.</p>
            </div>
        </div> <!--delivered container end-->
        <div class="location-container">
            <div class="location-title">
                <h6 class="title-min">locations</h6>
                <h1 class="title-medium">Visit our Bakeries</h1>
            </div>
            <div class="location-image-container">
                <div class="image-container">
                    <img src="../assets/images/new-york-bk-1200x794.jpg" alt="New York Bakery">
                    <div class="newyork-container">
                        <div class="title">
                            <h1>New York</h1>
                        </div>
                        <div class="time-container">
                            <div>
                                <h6>call us</h6>
                                <h6>1.800.458.556</h6>
                            </div>
                            <div>
                                <h6>open all week</h6>
                                <h6>9:00 am - 6:00 pm</h6>
                            </div>
                            <div>
                                <h5>View map</h5>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="image-container">
                    <img src="../assets/images/london-bk-1200x794.jpg" alt="">
                    <div class="london-container">
                        <div>
                            <h1>London</h1>
                        </div>
                        <div class="time-container">
                            <div>
                                <h6>call us</h6>
                                <h6>1.800.458.556</h6>
                            </div>
                            <div>
                                <h6>open all week</h6>
                                <h6>9:00 am - 6:00 pm</h6>
                            </div>
                            <div>
                                <h5>View map</h5>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div> <!--location container end-->
    </main>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.moments-container {
    height: 110vh;
}

.moments-title-container {
    margin: 0 auto;
    width: 30vw;
    height: 20vh;
    text-align: center;
}

.title-min {
    padding-bottom: 20px;
    text-transform: uppercase;
    font-weight: 100;
}

.moments-title-container h1 {
    color: $secondary-color;
}

.moments-image-container {
    height: 90vh;
}

.moments-image-container img {
    width: 43vw;
}


.product-container {
    height: 80vh;
    width: 90vw;
    margin: 0 auto;
}

.product-text {
    width: 30%;
    height: 50%;
    text-align: center;
}

.product-image-container {
    background-color: red;
    height: 50%;

    img {
        height: 100%;
    }
}

.product-text {

    h1 {
        color: $secondary-color;
    }

    button {
        padding: 15px 25px;
        border-radius: 7px;
        border-style: none;
        background-color: $secondary-color;
        color: white;
        font-weight: bold;
    }

    p {
        color: black;
        line-height: 35px;
        font-weight: 100;
        margin: 20px 0;
    }
}

.tell-us-container {
    background-image: url(../assets/images/bakery-process-1.jpg);
    background-size: contain;
    background-repeat: no-repeat;
    width: 90vw;
    height: 70vh;
    margin: 5vh auto;

    h1 {
        padding: 100px;
        color: white;
        font-size: 4rem;
        font-weight: bolder;
        max-width: 900px;
    }

    h2 {
        float: right;
        padding: 100px;
        color: white;
        font-size: 7rem;
        max-width: 900px;
        font-weight: 100;
    }
}

.tell-us-text {
    width: 30vw;
    margin-left: 65%;
    margin-top: 80px;
}

p,
h1,
h2,
h3,
h4 {
    color: white;
}

h3 {
    text-transform: uppercase;
    font-size: 0.8rem;
}

p {
    font-size: 1.2rem;
}

.we-start-container {
    width: 90vw;
    height: 70vh;
    margin: 0 auto;
}

.we-start-image {
    background-image: url(../assets/images/bakery-process-2.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    width: 44vw;
    height: 100%;

    div {
        padding: 0 50px;
    }

    h1 {
        padding: 50px 0;
        font-size: 4rem;
    }

    h2 {
        padding-top: 20px;
        margin-left: 80px;
        font-size: 7rem;
        font-weight: 100;
    }

}

.we-start-text {
    width: 44vw;
    height: 100%;

    div {
        width: 68%;
        height: 70%;
        margin: 100px auto;
    }

    h5 {
        color: $secondary-color;
        font-size: 30px;
        line-height: 45px;
        padding: 30px 0;
    }

    h6 {
        font-weight: 300;
    }

}



.we-start-image-text {
    width: 400px;
    margin-left: 80px;
    margin-top: 250px;
}



.delivered-container {
    background-image: url(../assets/images/bakery-process-3.jpg);
    background-size: contain;
    background-repeat: no-repeat;
    width: 90vw;
    height: 70vh;
    margin: 7vh auto;
}

.delivered-title {
    width: 85%;
    height: 20%;
    margin: 0 auto;

    h1 {
        font-size: 4rem;
        padding-top: 50px;
    }

    h2 {
        font-size: 7rem;
        font-weight: 100;
        padding-top: 20px;
    }

}

.delivered-text {
    width: 30%;
    height: 30%;
    margin-top: 15%;
    margin-left: 120px;
}



.location-container {
    width: 90vw;
    min-height: 50vh;
    margin: 20vh auto;
}

.location-title {
    width: 20%;
    height: 100px;
    margin: 0 auto;
    text-align: center;

    h6 {
        text-transform: uppercase;
        color: $secondary-color;
        font-weight: 100;
        font-size: 0.75rem;
    }

    h1 {
        color: $secondary-color;
    }
}

.location-image-container {
    width: 100%;
    min-height: 800px;
}

.image-container {
    width: calc(100% / 2);
    height: 500px;
}



.location-image-container img {
    width: 100%;
}

.newyork-container {
    width: 100%;
    height: 200px;
}

.london-container {
    width: 100%;
    height: 200px;
}

.newyork-container,
.london-container {

    h1 {
        color: $secondary-color;
        text-align: center;
        padding-top: 20px;
    }
}


.time-container {
    width: 90%;
    height: 100px;
    margin: 0 auto;

    div {
        width: calc(100% / 3);
        height: 50px;
        margin-top: 20px;
    }

    h6 {
        text-align: center;
        text-transform: uppercase;
        font-size: 0.8rem;
    }

    h5 {
        color: $secondary-color;
        font-size: 0.8rem;
        text-align: center;
        cursor: pointer;
    }
}

.cookie-container {
    align-items: center;
    width: 100%;
    height: 110vh;
}

.moments-image-container {
    display: flex;
    justify-content: space-evenly;
}

.product-container {
    align-items: center;
}

.product-text {
    display: flex;
    flex-direction: column;
    gap: 3px;
    padding: 4px;
    align-items: center;
    justify-content: center;
}

.we-start-text {
    flex-direction: column;
    background-color: $third-color
}

.location-image-container,
.cookie-image-container,
.we-start-container,
.time-container,
.location-image-container,
.cookie-image-container,
.we-start-container,
.time-container,
.delivered-title,
.product-container,
.cookie-container,
.we-start-text,
.tell-us-container div,
.we-start-image div {
    @include my-display-flex-1();
}



.site-main {
    width: 100%;
    min-height: 800vh;
}



.cookie-text {
    width: 30vw;
    height: 70vh;
    margin-left: 150px;

    button {
        padding: 15px 25px;
        border-radius: 7px;
        border-style: none;
        background-color: $secondary-color;
        color: white;
        font-weight: bold;
        margin-top: 50px;
    }

}

.cookie-image-container {
    width: 50vw;
    height: 70vh;
    margin-right: 150px;
}

.cookie-image-container img {
    height: 70vh;
}

.title-medium {
    font-size: 30px;
    line-height: 40px;
    color: $secondary-color;
}
</style>