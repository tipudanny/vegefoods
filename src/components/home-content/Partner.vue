<template>
    <section class="ftco-section ftco-partner">
        <div class="container">
            <div class="row">
                <div v-for="partner in partners" class="col-sm ftco-animate">
                    <a href="#" class="partner">
                        <img
                            :src="partner.image"
                            class="img-fluid"
                            alt="Colorlib Template"
                        />
                    </a>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
    name: "Partner",
        mounted() {
        },
        data(){
            return{
                partners:[
                    { image:'assets/images/partner-1.png'},
                    { image:'assets/images/partner-2.png'},
                    { image:'assets/images/partner-3.png'},
                    { image:'assets/images/partner-4.png'},
                    { image:'assets/images/partner-5.png'},
                ]
            }
        }
    }
</script>

<style scoped>

</style>