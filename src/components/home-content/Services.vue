<template>
    <div>
        <section class="ftco-section">
            <div class="container">
                <div class="row no-gutters ftco-services">
                    <div
                        v-for="service in services"
                        class="col-md-3 text-center d-flex align-self-stretch ftco-animate">
                        <div class="media block-6 services mb-md-0 mb-4">
                            <div
                                class="icon bg-color-1 active d-flex justify-content-center align-items-center mb-2"
                            >
                                <span :class="service.icon"></span>
                            </div>
                            <div class="media-body">
                                <h3 class="heading">{{ service.name}}</h3>
                                <span>{{ service.description}}</span>
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
    name: "Services",
    mounted() {
    },
    data(){
        return{
            services:[
                {
                    name:'Free Shipping',
                    description:'On order over $100',
                    icon:'flaticon-shipped'
                },
                {
                    name:'Always Fresh',
                    description:'Product well package',
                    icon:'flaticon-diet'
                },
                {
                    name:'Superior Quality',
                    description:'Quality Products',
                    icon:'flaticon-award'
                },
                {
                    name:'Support',
                    description:'24/7 Support',
                    icon:'flaticon-customer-service'
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