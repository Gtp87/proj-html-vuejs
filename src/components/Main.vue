<template>
<main>
    <div class="container-50">
        <div class="main-title text-center pt-5">
            <h6 class="text-uppercase font-monospace">phasellus eget metus</h6>
            <h3 class="fw-bold">All the latest news</h3>
        </div>
    </div>
    <div class="container-70">
        <CardNews />
        <div class="featured-article mt-5">
            <div class="feat-article-text text-light">
                <h6 class="text-uppercase font-monospace">featured article</h6>
                <h4 class="fw-bold fs-2">Cras malesuada et orci eget pharetra</h4>
                <p>In quis lectus sed leo elementum faucibus in dapibus dictum. Nullamolestie tortor nec lectus veneratis, sed blandit dui, dolor at bibendum sadips ets ipsums dolore ficilis uns leo lectus.</p>
                <button type="button" class="btn btn-dark">READ MORE ></button>
            </div>
        </div>
        <CardFeatured />
        <div class="row review mt-4 mb-4 pt-4">
            <div class="col-8">
                <div class="reviewed-product mt-2">
                    <div class="reviewed-product-text text-light">
                        <h6 class="text-uppercase font-monospace">reviewed product</h6>
                        <h4 class="fs-2 fw-bold">Mauris viverra atisan ipsus eget felis prims efficitur varius</h4>
                        <p>In quis lectus sed leo elementum faucibus in dapibus dictum. Nullamolestie tortor nec lectus veneratis, sed blandit dui, dolor at bibendum.</p>
                        <button type="button" class="btn btn-dark">READ MORE ></button>
                    </div>
                </div>
            </div>
            <CardTutorial />
        </div>
    </div>
    <div class="blog text-uppercase text-light text-center">
        <div class="blog-text">
            <h5> read our blog <i class="fas fa-long-arrow-alt-right"></i></h5>
        </div>
    </div>
    <div class="forum-section">
        <div class="container-70">
            <div class="forum-title text-center pt-5 pb-5">
                <h6 class="text-uppercase font-monospace">phasellus eget metus</h6>
                <h3 class="fw-bold pb-4">Forum Sections</h3>
            </div>
            <div class="forum-cards mt-4">
                <ForumCards />
            </div>
        </div>
    </div>
    <div class="blog text-uppercase text-light text-center">
        <div class="blog-text">
            <h5> go to our forum <i class="fas fa-long-arrow-alt-right"></i></h5>
        </div>
    </div>
    <div class="community">
        <div class="container-50 community-text text-center">
            <h2 class="fw-bold fs-1">Hey! Join to our <br> Community</h2>
            <p>Nulla molestie tortor nec lectus venenatis, sed blandit dui finibus. Curabitur feugiat <br> vulputate purus ipsum dolores ficilis uns etra</p>
            <button type="button" class="btn btn-primary">SIGN UP > </button>
        </div>
    </div>
    <div class="subscribe">
        <div class="text-center">
            <h4>Subscribe to our Newsletter</h4>
            <div class="search-container w-100 mt-4 pt-3">
                    <input class="w-25" placeholder="Insert your email*" type="text">
                    <button class="btn btn-dark ms-3 w-10" type="submit">SEND</button>
                </div>
        </div>
    </div>
</main>
</template>

<script>
import ForumCards from './ForumCards.vue';
import CardNews from './CardNews.vue';
import CardFeatured from './CardFeatured.vue';
import CardTutorial from './CardTutorial.vue';
export default {
    name: "Main",
    components: {
        ForumCards,
        CardNews,
        CardFeatured,
        CardTutorial,
    }

}
</script>

<style lang="scss">
@import "../assets/scss/style.scss";

.main-title h6 {
    font-size: 0.8em;
    font-weight: bold;
}
.main-title::after {
    height: 3px;
    width: 10%;
    margin: auto;
    display: block;
    background-color: $colorSalmon;
    content:"";
}

.img-container {
    width: 100%;
    img {
        width: 100%;
    }
}
.news-title {
    font-size: 0.9em;
    font-weight: bold;
    margin-top: 0.6em;
}

.news-date {
    font-size: 0.6em;
    font-weight: lighter;
    margin-bottom: 0.9em;
}

.news-text {
    font-size: 0.7em;
    font-weight: lighter;
}

.featured-article {
    background-image: url(../assets/img/featured_article_1_bg.jpg);
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    .feat-article-text {
        padding: 20% 10% 10% 5%;
    }
    .btn-dark {
        background-color: $sharkBlack;
        border-color: $sharkBlack; 
    }

}

.review {
    padding-bottom: 8em;
    .reviewed-product {
        background-image: url(../assets/img/featured_article_2_bg.jpg);
        height: 58vh;
        background-position: center;
        background-size: cover;
        background-repeat: no-repeat;
        .reviewed-product-text {
            padding: 20% 10% 10% 5%;
            h6 {
                font-size: 0.8em;
                font-weight: bold;
            }
            .btn-dark {
            background-color: $sharkBlack;
            border-color: $sharkBlack; 
            }
        }
    }
}


.tutorials::after {
    height: 3px;
    width: 10%;
    display: block;
    background-color: $colorSalmon;
    content:"";
}

.blog {
    background-color: $sharkBlack;
    height: 100px;
    position: relative;
    .blog-text {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    cursor: pointer;
    }
}

.forum-title::after {
    height: 3px;
    width: 10%;
    margin: auto;
    display: block;
    background-color: $colorSalmon;
    content:"";
}

.forum-section {
    background-color: $silverChalice;
    padding-bottom: 8em;
    h6 {
    font-size: 0.8em;
    font-weight: bold;
}
}
.card-container {
    background-color: $colorWhite;
    width: 200px;
    height: 200px;
    border-top: 2px solid #27aabe;
    cursor: pointer;
    .icon-cont {
        width: 84px;
        height: 84px;
        line-height: 84px;
        font-size: 42px;
        border-radius: 100%;
        margin: 0 auto;
        background-color: $colorSalmon;
        color: $colorWhite;
    }
}

.community {
    position: relative;
    background-image: url(../assets/img/join_now_cta_bg.jpg);
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;  
    height: 400px;  
    color: $colorWhite;
    .community-text {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        .btn-primary {
            background-color: $colorMalibu;
            border-color: $colorMalibu;  
        }
    }    
}

.subscribe {
    background-color: $silverChalice;
    height: 200px;
    padding-top: 8em;
    padding-bottom: 15em;
    input {
        padding: 0.4em;
        outline: none;
        border: none;
    }
}
</style>