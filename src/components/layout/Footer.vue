<template>
    <footer class="ftco-footer ftco-section">
        <div class="container">
            <div class="row">
                <div class="mouse">
                    <a href="#" class="mouse-icon">
                        <div class="mouse-wheel">
                            <span class="ion-ios-arrow-up"></span>
                        </div>
                    </a>
                </div>
            </div>
            <div class="row mb-5">
                <div class="col-md">
                    <div class="ftco-footer-widget mb-4">
                        <h2 class="ftco-heading-2">{{ wdget_vegefoods.title}}</h2>
                        <p>{{ wdget_vegefoods.description}}</p>
                        <ul class="ftco-footer-social list-unstyled float-md-left float-lft mt-5">
                            <li class="ftco-animate">
                                <a href="#"><span class="icon-twitter"></span></a>
                            </li>
                            <li class="ftco-animate">
                                <a href="#"><span class="icon-facebook"></span></a>
                            </li>
                            <li class="ftco-animate">
                                <a href="#"><span class="icon-instagram"></span></a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="col-md">
                    <div class="ftco-footer-widget mb-4 ml-md-5">
                        <h2 class="ftco-heading-2">Menu</h2>
                        <ul class="list-unstyled">
                            <li v-for="menu in wdget_menus">
                                <a href="#" class="py-2 d-block">{{ menu.menu}}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="ftco-footer-widget mb-4">
                        <h2 class="ftco-heading-2">Help</h2>
                        <div class="d-flex">
                            <ul class="list-unstyled mr-l-5 pr-l-3 mr-4">
                                <li v-for="help in wdget_help">
                                    <a href="#" class="py-2 d-block">{{ help.help}}</a>
                                </li>
                            </ul>
                            <ul class="list-unstyled">
                                <li><a href="#" class="py-2 d-block">FAQs</a></li>
                                <li><a href="#" class="py-2 d-block">Contact</a></li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="col-md">
                    <div class="ftco-footer-widget mb-4">
                        <h2 class="ftco-heading-2">Have a Questions?</h2>
                        <div class="block-23 mb-3">
                            <ul>
                                <li>
                                    <span class="icon icon-map-marker"></span>
                                    <span class="text"> {{ wdget_questions.location }}</span>
                                </li>
                                <li>
                                    <a href="#">
                                        <span class="icon icon-phone"></span>
                                        <span class="text">{{ wdget_questions.phone }}</span>
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        <span class="icon icon-envelope"></span>
                                        <span class="text">{{ wdget_questions.email }}</span>
                                    </a>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
            <div class="row">
                <div class="col-md-12 text-center">
                    <p>
                        <!-- Link back to Colorlib can't be removed. Template is licensed under CC BY 3.0. -->
                        Copyright &copy;
                        {{ currentYear }}
                        All rights reserved | This template is made with
                        <i class="icon-heart color-danger" aria-hidden="true"></i> by
                        <a href="https://colorlib.com" target="_blank">Colorlib</a>
                        <!-- Link back to Colorlib can't be removed. Template is licensed under CC BY 3.0. -->
                    </p>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
    export default {
        name: "Footer",
        mounted() {
            this.currentYear = new Date().getFullYear()
        },
        data(){
            return{
                currentYear:'',
                wdget_vegefoods:{
                    title:'Vegefoods',
                    description:'Far far away, behind the word mountains, far from the countries Vokalia and Consonantia.'
                },
                wdget_menus:[
                    {menu:'Shop'},
                    {menu:'About'},
                    {menu:'Journal'},
                    {menu:'Contact Us'},
                ],
                wdget_help:[
                    {help:'Shipping Information'},
                    {help:'Returns & Exchange'},
                    {help:'Terms & Conditions'},
                    {help:'Privacy Policy'},
                ],
                wdget_questions:{
                    location:'203 Fake St. Mountain View, San Francisco, California,USA',
                    phone:'+2 392 3929 210',
                    email:'info@yourdomain.com'
                },
            }
        }
    }
</script>

<style scoped>

</style>