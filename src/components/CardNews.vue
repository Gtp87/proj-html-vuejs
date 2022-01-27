<template>
<div class="row row-cols-3 mt-5">
    <div class="col news"
    v-for="(card,index) in news"
    :key="index + 'news'">
        <div class="img-container">
            <img :src="card.img" alt="">
        </div>
        <div class="news-article">
            <div class="news-title">{{card.title}}</div>
            <div class="news-date"><span>{{card.date}}</span> |<span class="fw-bold"> {{card.comments}}</span></div>
            <div class="news-text">{{card.text}}</div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name: 'CardNews',
    data() {
        return{
            news: [
                {
                    img: require('../assets/img/post_feat_img_25-320x202.jpg'),
                    title: 'Morbi vitae dui euismod vulputate sollicitudin',
                    date: 'October 11th, 2015',
                    comments: '2 Comments',
                    text: 'Donec finibus sit amet orci eget ulticies. Praesent posuere ante ut erat fringilla, vestibulum placerat metus mattis. Aenean dictum vitae nisl'
                },
                {
                    img: require('../assets/img/post_feat_img_24-320x202.jpg'),
                    title: 'Vivamus pellenteque, felis quis varius',
                    date: 'October 11th, 2015',
                    comments: 'Comments Off',
                    text: 'Donec finibus sit amet orci eget ulticies. Praesent posuere ante ut erat fringilla, vestibulum placerat metus mattis. Aenean dictum vitae nisl'
                },
                {
                    img: require('../assets/img/post_feat_img_23-320x202.jpg'),
                    title: 'Donec ornare pretium eget scelisque justo',
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