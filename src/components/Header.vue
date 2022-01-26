<template>
<header>
    <div class="container-70">
        <div class="row">
            <div class="col-12 d-flex justify-content-between">
                <div class="logo">
                    <img src="../assets/img/logo.png" alt="logo">
                </div>
                <div class="d-flex align-items-center">
                    <ul class="list-unstyled mt-3">
                        <li><a href="#">Home</a></li>
                        <li><a href="#">Apple</a></li>
                        <li><a href="#">Microsoft</a></li>
                        <li><a href="#">Android</a></li>
                        <li><a href="#">Forums</a></li>
                        <li><a href="#">Contact us</a></li>
                        <li><button type="button" class="my_btn btn btn-dark">JOIN US</button></li>
                        <li><i class="fas fa-search"></i></li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
        <div class="jumbo-container-top">
            <div class="container-70">
                <div class="jumbo-text-top">
                    <h1 class="display-1 fw-bold">Tech Forum!</h1>
                    <p>Discuss all the latest technology news and trends</p>
                    <button type="button" class="btn btn-primary">GET AVADA NOW! > </button>
                </div>
            </div>
        </div>
        <div class="jumbo-container-bottom">
            <div class="container-50">
                <div class="jumbo-text-bottom text-center">
                    <h6 class="text-uppercase font-monospace">avada forum is the place to be</h6>
                    <h5 class="fw-light fs-5 lh-base">In qui lectus sed leo elementum faucibus in dapibus dictum. <br> Nulla molestie tortor nec lectus venenatis, sed blandit dui finibus. <br> dolor at, bibendum purus. Donec vehicula nec tortor ac finibus</h5>
                </div>
            </div>
        </div>
</header>
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style lang="scss">
@import "../assets/scss/style.scss";

header {
    color: white;
    background-color: $colorMalibu;
    .logo {
    padding: 0.6em;
    cursor: pointer;
    }
    li {
        display: inline-block;
        margin: 0 1em;
        cursor: pointer;
        .my_btn {
            width: 100px;
            padding: 0.5em;
        }
        a {
            text-decoration: none;
            color: $colorWhite;
        }
    }
    
    .jumbo-container-top {
        background-image: url(../assets/img/home_slider_bg.jpg);
        background-position: center;
        background-size: cover;
        background-repeat: no-repeat;
        .jumbo-text-top {
            padding-top: 20%;
            padding-bottom: 20%;
            .btn-primary {
            background-color: $colorMalibu;
            border-color: $colorMalibu;  
            }
        }
    }
    .jumbo-container-bottom {
        background-color: $silverChalice;
        color: black;
        .jumbo-text-bottom {
            padding: 4em 0;
            h6 {
                font-size: 0.8em;
                font-weight: bold;
            }
        }
    }
}

</style>