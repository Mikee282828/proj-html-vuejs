<script>
export default {
    data() {
        return {

        }
    },
    props: {
        cardInfo: Array
    },
    methods: {
        getSvg(name) {
            return new URL(`../../assets/svg/${name}`, import.meta.url).href;
        }
    }
}
</script>

<template>
    <div class="bkg_fafafa">
        <div class="container pt-3 pb-5">
            <!-- title -->
            <div class="my_title">
                <h1 class="text-center">Our specialties <span class="text-danger">.</span></h1>
                <p class="text-center">Lorem ipsum dolor sit amet consectetur adipisicing elit</p>
                <div class="my_separator"></div>
            </div>
            <!-- specialties cards -->
            <div class="row">
                <div class="col-3 text-center" v-for="element in cardInfo">
                    <img class="mb-3" :src="getSvg(element.img)" alt="">
                    <h5>{{ element.title }}</h5>
                    <p>Lorem, ipsum dolor sit amet consect</p>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.container {
    background-color: #FFFFFF;
}

.bkg_fafafa {
    background-color: #FAFAFA;
    color: black;
}

.my_separator {
    border: solid 0.1rem #FF4612;
    width: 5rem;
    position: relative;
    left: 50%;
    transform: translate(-50%, 0);
}
</style>