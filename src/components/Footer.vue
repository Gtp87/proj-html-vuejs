<template>
<footer>
    <FooterTop />
    <div class="bottom mt-5">
        <div class="container-70">
            <div class="footer-bottom mt-3">
                <div class="col-12 d-flex justify-content-between">
                    <div class="copyright pt-4">
                        &#169; Copyright 2012 - 2020 | Avada Theme by <span class="fw-bold">ThemeFusion</span> | All Rights Reserved | Powered by <span class="fw-bold">WordPress</span>
                    </div>
                    <div class="d-flex align-items-center">
                        <ul class="list-unstyled list-inline mt-3">
                            <li class="list-inline-item">
                                <div class="facebook icon-container text-center">
                                    <i class="fab fa-facebook-f"></i>
                                </div>
                            </li>
                            <li class="list-inline-item">
                                <div class="twitter icon-container text-center">
                                    <i class="fab fa-twitter"></i>
                                </div>
                            </li>
                            <li class="list-inline-item ">
                                <div class="instagram icon-container text-center">
                                    <i class="fab fa-instagram"></i>
                                </div>
                            </li>
                            <li class="list-inline-item">
                                <div class="youtube icon-container text-center">
                                    <i class="fab fa-youtube"></i>
                                </div>
                            </li>
                        </ul>
                    </div>

                </div>
            </div>
        </div>
    </div>
</footer>
</template>

<script>
import FooterTop from './FooterTop.vue';
export default {
    name: "Footer",
    components: {
        FooterTop,
    },
}
</script>

<style lang="scss">
@import "../assets/scss/style.scss";
@import "../assets/scss/partials/_variables.scss";
.link {
    border-bottom: 2px solid $silverChalice;
    font-weight: bold;
    cursor: pointer;
    &:hover {
    color: $colorMalibu;
    }
}

.forum-text,
.link {
    font-size: 0.9em;
}
.bottom::before {
    height: 2px;
    width: 97%;
    margin: auto;
    display: block;
    background-color: $silverChalice;
    content:"";
}

.footer-bottom {
    .copyright {
        font-size: 0.6em;
    }
    .icon-container {
        width: 30px;
        height: 30px;
        line-height: 30px;
        font-size: 15px;
        border-radius: 100%;
        margin: 0 auto;
        color: $colorWhite;
        font-size: 0.9em;
        cursor: pointer;
    }

    .icon-container:hover {
        opacity: 0.4;
    }
    .facebook {
        background-color: $colorUltramarine;
    }
    .twitter {
        background-color: $colorMalibu;
    }
    .instagram {
        background-color: $royalBlue;
    }
    .youtube {
        background-color: $totemPole;
    }
}
</style>