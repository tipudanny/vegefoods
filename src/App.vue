<template>
    <div id="app">
        <TopMenu />
        <Nav />
        <router-view/>
        <Footer/>
        <!-- loader -->
        <div id="ftco-loader" class="show fullscreen">
            <svg class="circular" width="48px" height="48px">
                <circle
                    class="path-bg"
                    cx="24"
                    cy="24"
                    r="22"
                    fill="none"
                    stroke-width="4"
                    stroke="#eeeeee"
                />
                <circle
                    class="path"
                    cx="24"
                    cy="24"
                    r="22"
                    fill="none"
                    stroke-width="4"
                    stroke-miterlimit="10"
                    stroke="#F96D00"
                />
            </svg>
        </div>
    </div>
</template>

<style>

</style>
<script>
import Nav from "./components/layout/Nav";
import TopMenu from "@/components/layout/TopMenu";
import Footer from "@/components/layout/Footer";
export default {
    components: {Footer, TopMenu, Nav}
}
</script>

<style scoped>

</style>