<template>
    <div>
        <section class="ftco-section ftco-category ftco-no-pt">
            <div class="container">
                <div class="row">
                    <div class="col-md-8">
                        <div class="row">
                            <div class="col-md-6 order-md-last align-items-stretch d-flex">
                                <div
                                    class="category-wrap-2 ftco-animate img align-self-stretch d-flex"
                                    :style="{'background-image': 'url('+centerProduct.image+')'}">
                                    <div class="text text-center">
                                        <h2>{{ centerProduct.title}}</h2>
                                        <p>{{ centerProduct.subtitle}}</p>
                                        <p><a href="#" class="btn btn-primary">Shop now</a></p>
                                    </div>
                                </div>
                            </div>
                            <div class="col-md-6">
                                <div
                                    v-for="(leftCat,index) in leftCategories" :key="index"
                                    class="category-wrap ftco-animate img d-flex align-items-end"
                                    :class="{ 'mb-4': index === 0 }"
                                    :style="{'background-image': 'url('+leftCat.image+')'}">
                                    <div class="text px-3 py-1">
                                        <h2 class="mb-0"><a href="#">{{ leftCat.name}}</a></h2>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="col-md-4">
                        <div
                            v-for="(rightCat,index) in rightCategories" :key="index"
                            class="category-wrap ftco-animate img d-flex align-items-end"
                            :class="{ 'mb-4': index === 0 }"
                            :style="{'background-image': 'url('+rightCat.image+')'}">
                            <div class="text px-3 py-1">
                                <h2 class="mb-0"><a href="#">{{ rightCat.name}}</a></h2>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>

<script>
export default {
    name: "Category",
    mounted() {
    },
    data(){
        return{
            leftCategories:[
                {
                    name:'Fruits',
                    image:'assets/images/category-1.jpg'
                },
                {
                    name:'Vegetables',
                    image:'assets/images/category-2.jpg'
                },
            ],
            centerProduct:{
                title:'Vegetables',
                subtitle:'Protect the health of every home',
                image:'assets/images/category.jpg'
            },
            rightCategories:[
                {
                    name:'Juices',
                    image:'assets/images/category-3.jpg'
                },
                {
                    name:'Dried',
                    image:'assets/images/category-4.jpg'
                },

            ],
        }
    },
    methods:{

    }
}
</script>

<style scoped>

</style>