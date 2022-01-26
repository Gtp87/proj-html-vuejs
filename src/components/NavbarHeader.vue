<template>
<div class="row">
    <div class="col-12 d-flex justify-content-between">
        <div class="logo">
            <img src="../assets/img/logo.png" alt="logo">
        </div>
        <div class="d-flex align-items-center">
            <ul class="list-unstyled mt-3">
                <li
                v-for="(element, index) in navbarItems"
                :key="index">
                <a 
                :href="element.url"
                >{{element.name}}</a>
                </li>
                <li><button type="button" class="my_btn btn btn-dark">JOIN US</button></li>
                <li><i class="fas fa-search"></i></li>
            </ul>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name: 'NavbarHeader',
    data() {
        return {
            navbarItems: [
                {
                    name: 'Home',
                    url: '#'
                },
                {
                    name: 'Apple',
                    url: '#'
                },
                {
                    name: 'Microsoft',
                    url: '#'
                },
                {
                    name: 'Android',
                    url: '#'
                },
                {
                    name: 'Forum',
                    url: '#'
                },
                {
                    name: 'Contact Us',
                    url: '#'
                }
            ]
        }
    }
}
</script>

<style lang='scss'>


</style>