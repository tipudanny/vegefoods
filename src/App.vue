<template>
    <div id="app">
        <TopMenu />
        <Nav />
        <router-view/>
    </div>
</template>

<style>

</style>
<script>
import Nav from "./components/layout/Nav";
import TopMenu from "@/components/layout/TopMenu";
export default {
    components: {TopMenu, Nav}
}
</script>