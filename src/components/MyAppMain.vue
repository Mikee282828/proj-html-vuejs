<script>
import store from "../data/store.js";
export default {
    name: "MyAppMain",
    data() {
        return {
            store
        }
    },
    methods: {
    },
    mounted() {
    }
}
</script>

<template>

    <h1>Questo è il main</h1>

    <Jumbotron />
    <Specialties />
    <Founder />
    <Events />
    <Stats />
    <News />
    <Testimonials />
    <Bigvideo />
    <Achievements />
    <Staff />
    <Contacts />
    <Plans />

</template>

<style scoped></style>
