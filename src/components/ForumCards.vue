<template>
<div class="row row-cols-4">
    <div class="col d-flex justify-content-center"
    v-for="(item,index) in cardItems"
    :key="index">
        <div class="card-container d-flex flex-column justify-content-center mb-4">
            <div class="icon-cont text-center">
                <i :class="item.class"></i>
            </div>
            <div class="card-text text-center mt-3">
                <h6 class="fs-6">{{item.text}}</h6>
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name: 'ForumCards',
    data() {
        return{
            cardItems: [
                {
                    class: 'far fa-file-alt',
                    text: 'News & Community'
                },
                {
                    class: 'fab fa-apple',
                    text: 'Apple Forum'
                },
                {
                    class: 'fab fa-windows',
                    text: 'Microsoft Forum'
                },
                {
                    class: 'fab fa-android',
                    text: 'Android Forum'
                },
                {
                    class: 'fas fa-coffee',
                    text: 'General Discussion'
                },
                {
                    class: 'fas fa-cubes',
                    text: 'Apps & Software'
                },
                {
                    class: 'fas fa-laptop',
                    text: 'Gadget & Stuff'
                },
                {
                    class: 'fas fa-wrench',
                    text: 'Tutorial & Guides'
                }
            ]
        }
    }

}
</script>

<style>

</style>