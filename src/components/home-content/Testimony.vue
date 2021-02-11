<template>
    <div>
        <section class="ftco-section testimony-section">
            <div class="container">
                <div class="row justify-content-center mb-5 pb-3">
                    <div class="col-md-7 heading-section ftco-animate text-center">
                        <span class="subheading">{{ header}}</span>
                        <h2 class="mb-4">{{ title}}</h2>
                        <p> {{ subtitle}}</p>
                    </div>
                </div>
                <div class="row ftco-animate">
                    <div class="col-md-12">
                        <div class="carousel-testimony owl-carousel">
                            <div v-for="testimonial in testimonials" class="item">
                                <div class="testimony-wrap p-4 pb-5">
                                    <div
                                        class="user-img mb-5"
                                        :style="{'background-image': 'url('+ testimonial.image+')'}"
                                    >
                                <span class="quote d-flex align-items-center justify-content-center">
                                  <i class="icon-quote-left"></i>
                                </span>
                                    </div>
                                    <div class="text text-center">
                                        <p class="mb-5 pl-4 line">
                                            {{ testimonial.description}}
                                        </p>
                                        <p class="name">{{ testimonial.name}}</p>
                                        <span class="position">{{ testimonial.designation}}</span>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        <hr />
    </div>
</template>

<script>
export default {
    name: "Testimony",
    mounted() {
    },
    data(){
        return{
            header:'Testimony',
            title:'Our satisfied customer says',
            subtitle:'Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts. Separated they live in',
            testimonials:[
                {
                    image:'assets/images/person_1.jpg',
                    description:'Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.',
                    name:'Garreth Smith',
                    designation:'Marketing Manager'
                },
                {
                    image:'assets/images/person_2.jpg',
                    description:'Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.',
                    name:'Garreth Smith',
                    designation:'Interface Designer'
                },
                {
                    image:'assets/images/person_3.jpg',
                    description:'Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.',
                    name:'Garreth Smith',
                    designation:'UI Designer'
                },
                {
                    image:'assets/images/person_1.jpg',
                    description:'Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.',
                    name:'Garreth Smith',
                    designation:'Web Developer'
                },
                {
                    image:'assets/images/person_1.jpg',
                    description:'Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.',
                    name:'Garreth Smith',
                    designation:'System Analyst'
                },


            ]
        }
    }
}
</script>

<style scoped>

</style>