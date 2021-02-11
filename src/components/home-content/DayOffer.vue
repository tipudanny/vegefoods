<template>
    <div>
        <section
            class="ftco-section img"
            :style="{'background-image': 'url('+ image+')'}">
            <div class="container">
                <div class="row justify-content-end">
                    <div
                        class="col-md-6 heading-section ftco-animate deal-of-the-day ftco-animate"
                    >
                        <span class="subheading">{{ headtext}}</span>
                        <h2 class="mb-4">{{ title}}</h2>
                        <p>
                            {{ description}}
                        </p>
                        <h3><a href="#">{{ name}}</a></h3>
                        <span class="price"> {{ basePrice}} <a href="#">now {{ offerPrice}} only</a></span>
                        <div id="timer" class="d-flex mt-5">
                            <div class="time" id="days"></div>
                            <div class="time pl-3" id="hours"></div>
                            <div class="time pl-3" id="minutes"></div>
                            <div class="time pl-3" id="seconds"></div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>

<script>
    export default {
        name: "DayOffer",
        data(){
            return{
                image:'assets/images/bg_3.jpg',
                headtext:'Best Price For You',
                title:'Deal of the day',
                description:'Far far away, behind the word mountains, far from the countries Vokalia and Consonantia',
                name:'Spinach',
                basePrice:'$10',
                offerPrice:'$5',

            }
        }
    }
</script>

<style scoped>

</style>