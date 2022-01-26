<template>
<div class="container-70">
    <div class="footer-top mt-5">
        <div class="row row-cols-4">
            <div class="col">
                <h6 class="text-uppercase fw-bold mb-4">avada tech forum</h6>
                <p class="forum-text pt-2">Sed semper, nisl id feugiat eleifend, erat est digssim felis, quis auctor elit enim nec ante. Cras et nibh risus. Pellentesque non mi sit amet mi intermentum</p>
            </div>
            <div class="col"
            v-for="(element,index) in footerCards"
            :key="index">
                <h6 class="text-uppercase fw-bold mb-4">{{element.title}}</h6>
                <div class="link pt-2 d-flex">
                    <span><i class="fas fa-chevron-right me-1"></i></span><p>{{element.links[0]}}</p>
                </div>
                <div class="link pt-2 d-flex">
                    <span><i class="fas fa-chevron-right me-1"></i></span><p>{{element.links[1]}}</p>
                </div>
                <div class="link pt-2 d-flex">
                    <span><i class="fas fa-chevron-right me-1"></i></span><p>{{element.links[2]}}</p>
                </div>
                <div class="link pt-2 d-flex">
                    <span><i class="fas fa-chevron-right me-1"></i></span><p>{{element.links[3]}}</p>
                </div>
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name: 'FooterTop',
    data(){
        return {
            footerCards: [
                {
                    title: 'popular topics',
                    links: [
                        'Nam a dolor voluptat massa auctor semper',
                        'Sed euismod nunc urna fermentum arcu dapibus fringilla',
                        'Cras lacinia tellus id mauris finibus lacus molestie',
                        'Curabitur a scelerisque ligula',
                    ]
                },
                {
                    title: 'recent topics',
                    links: [
                        'Cras lacinia tellus id mauris finibus lacus molestie',
                        'Proin at ligula sagittis vestibulum nisi vitae',
                        'Sed nec metus at est tincidunt elementum',
                        'Nulla egestas nulla eu nulla suscipit molestie',
                    ]
                },
                {
                    title: 'last replies',
                    links: [
                        'Cras lacinia tellus id mauris finibus lacus molestie',
                        'Cras lacinia tellus id mauris finibus lacus molestie',
                        'Nulla egestas nulla eu nulla suscipit molestie',
                        'Mauris ac nibh quis eros sagittis lacinia a et dui',
                    ]
                }
            ],
        }
    },
}
</script>

<style>

</style>