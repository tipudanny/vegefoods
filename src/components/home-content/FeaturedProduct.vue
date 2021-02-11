<template>
    <div>
        <section class="ftco-section">
            <div class="container">
                <div class="row justify-content-center mb-3 pb-3">
                    <div class="col-md-12 heading-section text-center ftco-animate">
                        <span class="subheading">{{ sectionInfo.sectionName}}</span>
                        <h2 class="mb-4">{{ sectionInfo.title}}</h2>
                        <p>
                            {{ sectionInfo.description}}
                        </p>
                    </div>
                </div>
            </div>
            <div class="container">
                <div class="row">
                    <div v-for="(product,index) in products " :key="index" class="col-md-6 col-lg-3 ftco-animate">
                        <div class="product">
                            <a href="#" class="img-prod">
                                <img
                                class="img-fluid"
                                :src="product.image"
                                alt="Colorlib Template"
                                />
                                <span v-if="product.offer != null" class="status">{{ product.offer}}</span>
                                <div class="overlay"></div>
                            </a>
                            <div class="text py-3 pb-4 px-3 text-center">
                                <h3><a href="#">{{ product.name}}</a></h3>
                                <div class="d-flex">
                                    <div class="pricing">
                                        <p v-if="product.offer != null" class="price">
                                            <span class="mr-2 price-dc">{{ product.basePrice}}</span>
                                            <span class="price-sale">{{ product.salePrice}}</span>
                                        </p>
                                        <p v-else class="price"><span>$120.00</span></p>
                                    </div>
                                </div>
                                <div class="bottom-area d-flex px-3">
                                    <div class="m-auto d-flex">
                                        <a href="#" class="add-to-cart d-flex justify-content-center align-items-center text-center">
                                            <span><i class="ion-ios-menu"></i></span>
                                        </a>
                                        <a href="#" class="buy-now d-flex justify-content-center align-items-center mx-1">
                                            <span><i class="ion-ios-cart"></i></span>
                                        </a>
                                        <a href="#" class="heart d-flex justify-content-center align-items-center">
                                            <span><i class="ion-ios-heart"></i></span>
                                        </a>
                                    </div>
                                </div>
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
    name: "FeaturedProduct",
    mounted() {
    },
    data(){
        return{
            sectionInfo:{
                sectionName:'Featured Products',
                title:'Our Products',
                description:'Far far away, behind the word mountains, far from the countries\n' + 'Vokalia and Consonantia',
            },
            products:[
                {
                    offer:'30%',
                    name:'Bell Pepper',
                    image:'/assets/images/product-1.jpg',
                    basePrice:'$120.00',
                    salePrice:'$80.00',
                },
                {
                    offer:null,
                    name:'Strawberry',
                    image:'/assets/images/product-2.jpg',
                    basePrice:'$120.00',
                    salePrice:null,
                },
                {
                    offer:null,
                    name:'Green Beans',
                    image:'/assets/images/product-3.jpg',
                    basePrice:'$120.00',
                    salePrice:null,
                },
                {
                    offer:null,
                    name:'Purple Cabbage',
                    image:'/assets/images/product-4.jpg',
                    basePrice:'$120.00',
                    salePrice:null,
                },
                {
                    offer:'30%',
                    name:'Tomatoe',
                    image:'/assets/images/product-5.jpg',
                    basePrice:'$120.00',
                    salePrice:'$80.00',
                },
                {
                    offer:null,
                    name:'Brocolli',
                    image:'/assets/images/product-6.jpg',
                    basePrice:'$120.00',
                    salePrice:null,
                },
                {
                    offer:null,
                    name:'Carrots',
                    image:'/assets/images/product-7.jpg',
                    basePrice:'$120.00',
                    salePrice:null,
                },
                {
                    offer:null,
                    name:'Fruit Juice',
                    image:'/assets/images/product-8.jpg',
                    basePrice:'$120.00',
                    salePrice:null,
                },
            ]
        }
    },
    methods:{

    }
}
</script>

<style scoped>

</style>