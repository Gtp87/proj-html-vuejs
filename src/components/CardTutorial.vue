<template>
<div class="col-4 d-flex flex-column">
    <div class="tutorials mb-4">
        <h5>Tutorials &amp; Guides</h5>
    </div>
    <div class="row pb-2"
    v-for="(tutorial,index) in tutorials"
    :key="index + 'tut'">
        <div class="col-6">
            <div class="img-container">
                <img :src="tutorial.img" alt="">
            </div>
        </div>
        <div class="col-6 news-article">
            <div class="news-title">{{tutorial.title}}</div>
            <div class="news-date"><span>{{tutorial.date}}</span> | <span class="fw-bold">{{tutorial.comments}}</span></div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name: 'CardTutorial',
    data(){
        return{
            tutorials:[
                {
                    img: require('../assets/img/post_feat_img_23-147x118.jpg'),
                    title: 'Donec ornare pretium eget scelisque justo',
                    date: 'October 11th, 2015',
                    comments: 'Comments Off',
                },
                {
                    img: require('../assets/img/post_feat_img_22-147x118.jpg'),
                    title: 'Fusce sollicitudin nunc sed placerat varius',
                    date: 'October 11th, 2015',
                    comments: 'Comments Off',
                },
                {
                    img: require('../assets/img/post_feat_img_20-147x118.jpg'),
                    title: 'Proin eu purus sed aru aliquet curabir vens',
                    date: 'October 11th, 2015',
                    comments: 'Comments Off',
                }
            ]
        }
    }

}
</script>

<style>

</style>