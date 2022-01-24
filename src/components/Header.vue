<template>
<header>
    <div class="container-70">
        <div class="row nav-menu">
            <div class="col-12 d-flex justify-content-between">
                <div class="logo">
                    <img src="../assets/img/logo.png" alt="logo">
                </div>
                <div class="d-flex align-items-center">
                    <ul class="list-unstyled mt-3">
                        <li>Home</li>
                        <li>Apple</li>
                        <li>Microsoft</li>
                        <li>Android</li>
                        <li>Forums</li>
                        <li>Contact us</li>
                        <li><button type="button" class="btn btn-dark">JOIN US</button></li>
                        <li><i class="fas fa-search"></i></li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
        <div class="jumbo-container">
            <div class="container-70">
                <div class="jumbo-text">
                    <h1 class="display-1">Tech Forum!</h1>
                    <p>Discuss all the latest technology news and trends</p>
                    <button type="button" class="btn btn-primary">GET AVADA NOW!</button>
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
    background-color: $headerBgColor;
    .container-70 {
        width: 70%;
        margin: auto;
    }
    .logo {
        padding: 0.6em;
    }
    li {
        display: inline-block;
        margin: 0 1em;
        cursor: pointer;
    }
    .jumbo-container {
        background-image: url(../assets/img/home_slider_bg.jpg);
        background-position: center;
        background-size: cover;
        background-repeat: no-repeat;
        .jumbo-text {
            padding-top: 30%;
            padding-bottom: 20%;
            .btn-primary {
            background-color: $headerBgColor;
            border-color: $headerBgColor;  
            }
        }
    }
}

</style>