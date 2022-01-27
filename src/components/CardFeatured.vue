<template>
<div class="row row-cols-3 mt-5">
    <div class="col news"
    v-for="(element,index) in featuredNews"
    :key="index + 'feat'">
        <div class="img-container">
            <img :src="element.img" alt="">
        </div>
        <div class="news-article">
            <div class="news-title">{{element.title}}</div>
            <div class="news-date"><span>{{element.date}}</span> |<span class="fw-bold"> {{element.comments}}</span></div>
            <div class="news-text">{{element.text}}</div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name: 'CardFeatured',
    data() {
        return{
            featuredNews: [
                {
                    img: require('../assets/img/post_feat_img_22-320x202.jpg'),
                    title: 'Fusce sollicitudibne nunc sed placerat varius',
                    date: 'October 11th, 2015',
                    comments: 'Comments Off',
                    text: 'Donec finibus sit amet orci eget ulticies. Praesent posuere ante ut erat fringilla, vestibulum placerat metus mattis. Aenean dictum vitae nisl'
                },
                {
                    img: require('../assets/img/post_feat_img_21-320x202.jpg'),
                    title: 'Donec facilis sodales leo sit amet laoreet',
                    date: 'October 11th, 2015',
                    comments: 'Comments Off',
                    text: 'Donec finibus sit amet orci eget ulticies. Praesent posuere ante ut erat fringilla, vestibulum placerat metus mattis. Aenean dictum vitae nisl'
                },
                {
                    img: require('../assets/img/post_feat_img_22-320x202.jpg'),
                    title: 'Proin eu purus sed aru aliquet curabir vens',
                    date: 'October 11th, 2015',
                    comments: 'Comments Off',
                    text: 'Donec finibus sit amet orci eget ulticies. Praesent posuere ante ut erat fringilla, vestibulum placerat metus mattis. Aenean dictum vitae nisl'
                }
            ]
        }
    }

}
</script>

<style>

</style>