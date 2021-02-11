<template>
    <div>
        <section id="home-section" class="hero">
            <div class="home-slider owl-carousel">

                <div
                    v-for="slide in sliders"
                    class="slider-item" :style="{'background-image': 'url('+ slide.image+')'}">
                    <div class="overlay"></div>
                    <div class="container">
                        <div
                            class="row slider-text justify-content-center align-items-center"
                            data-scrollax-parent="true"
                        >
                            <div class="col-md-12 ftco-animate text-center">
                                <h1 class="mb-2">{{ slide.title}}</h1>
                                <h2 class="subheading mb-4">
                                    {{ slide.subtitle }}
                                </h2>
                                <p><a href="#" class="btn btn-primary">View Details</a></p>
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
    name: "OwlCarousel",
    mounted() {
    },
    data(){
        return{
            sliders:[
                {
                    image:'assets/images/bg_1.jpg',
                    title:'We serve Fresh Vegestables &amp; Fruits',
                    subtitle:'We deliver organic vegetables &amp; fruits'
                },
                {
                    image:'assets/images/bg_2.jpg',
                    title:'100% Fresh &amp; Organic Foods',
                    subtitle:'We deliver organic vegetables &amp; fruits'
                },

            ]
        }
    }
}
</script>

<style scoped>

</style>