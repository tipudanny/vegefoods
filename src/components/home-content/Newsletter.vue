<template>
    <section class="ftco-section ftco-no-pt ftco-no-pb py-5 bg-light">
        <div class="container py-4">
            <div class="row d-flex justify-content-center py-5">
                <div class="col-md-6">
                    <h2 style="font-size: 22px" class="mb-0">
                        {{ title}}
                    </h2>
                    <span> {{ subtitle}}</span>
                </div>
                <div class="col-md-6 d-flex align-items-center">
                    <form action="#" class="subscribe-form">
                        <div class="form-group d-flex">
                            <input
                                type="text"
                                class="form-control"
                                placeholder="Enter email address"
                                v-model="email"
                            />
                            <input type="submit" value="Subscribe" class="submit px-3" />
                        </div>
                    </form>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "Newsletter",
    mounted() {
    },
    data(){
        return{
            title:'Subcribe to our Newsletter',
            subtitle: 'Get e-mail updates about our latest shops and special offers',
            email:''

        }
    }
}
</script>

<style scoped>

</style>