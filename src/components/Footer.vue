<template>
<footer>
    <div class="container-70">
        <div class="footer-top mt-5">
            <div class="row row-cols-4">
                <div class="col">
                    <h6 class="text-uppercase fw-bold mb-4">avada tech forum</h6>
                    <p class="forum-text pt-2">Sed semper, nisl id feugiat eleifend, erat est digssim felis, quis auctor elit enim nec ante. Cras et nibh risus. Pellentesque non mi sit amet mi intermentum</p>
                </div>
                <div class="col">
                    <h6 class="text-uppercase fw-bold mb-4">popular topics</h6>
                    <div class="link pt-2 d-flex">
                        <span><i class="fas fa-chevron-right me-1"></i></span><p>Nam a dolor voluptat massa auctor semper</p>
                    </div>
                    <div class="link pt-2 d-flex">
                        <span><i class="fas fa-chevron-right me-1"></i></span><p>Sed euismod nunc urna fermentum arcu dapibus fringilla</p>
                    </div>
                    <div class="link pt-2 d-flex">
                        <span><i class="fas fa-chevron-right me-1"></i></span><p>Cras lacinia tellus id mauris finibus lacus molestie</p>
                    </div>
                    <div class="link pt-2 d-flex">
                        <span><i class="fas fa-chevron-right me-1"></i></span><p>Curabitur a scelerisque ligula</p>
                    </div>
                </div>
                <div class="col">
                    <h6 class="text-uppercase fw-bold mb-4">recent topics</h6>
                    <div class="link pt-2 d-flex">
                        <span><i class="fas fa-chevron-right me-1"></i></span><p>Cras lacinia tellus id mauris finibus lacus molestie</p>
                    </div>
                    <div class="link pt-2 d-flex">
                        <span><i class="fas fa-chevron-right me-1"></i></span><p>Proin at ligula sagittis vestibulum nisi vitae</p>
                    </div>
                    <div class="link pt-2 d-flex">
                        <span><i class="fas fa-chevron-right me-1"></i></span><p>Sed nec metus at est tincidunt elementum</p>
                    </div>
                    <div class="link pt-2 d-flex">
                        <span><i class="fas fa-chevron-right me-1"></i></span><p>Nulla egestas nulla eu nulla suscipit molestie</p>
                    </div>
                </div>
                <div class="col">
                    <h6 class="text-uppercase fw-bold mb-4">latest replies</h6>
                    <div class="link pt-2 d-flex">
                        <span><i class="fas fa-chevron-right me-1"></i></span><p>Cras lacinia tellus id mauris finibus lacus molestie</p>
                    </div>
                    <div class="link pt-2 d-flex">
                        <span><i class="fas fa-chevron-right me-1"></i></span><p>Cras lacinia tellus id mauris finibus lacus molestie</p>
                    </div>
                    <div class="link pt-2 d-flex">
                        <span><i class="fas fa-chevron-right me-1"></i></span><p>Nulla egestas nulla eu nulla suscipit molestie</p>
                    </div>
                    <div class="link pt-2 d-flex">
                        <span><i class="fas fa-chevron-right me-1"></i></span><p>Mauris ac nibh quis eros sagittis lacinia a et dui</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
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
export default {
    name: "Footer"

}
</script>

<style lang="scss">
@import "../assets/scss/style.scss";
@import "../assets/scss/partials/_variables.scss";
.link {
    border-bottom: 2px solid $silverChalice;
    font-weight: bold;
    cursor: pointer;
}

.link:hover {
    color: $colorMalibu;
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