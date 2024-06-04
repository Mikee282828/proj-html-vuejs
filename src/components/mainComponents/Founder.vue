<script>
export default {
    name: "Founder",
    props: {
        foundersImg: Array
    },
    methods: {
        getSvg(name, isSvg) {
            if (isSvg) {
                return new URL(`../../assets/svg/${name}`, import.meta.url).href;
            } else {
                return new URL(`../../assets/img/${name}`, import.meta.url).href;
            }
        }
    }
}
</script>

<template>
    <!-- ancora da mettere responsive -->
    <div class="bkg_fafafa py-5">
        <div class="my_container">
            <div class="row justify-content-center align-items-center g-0">
                <div class="col-5 my_cardLx">
                    <div class="my_carousel w-100" v-for="element, index in foundersImg">
                        <img :src="getSvg(element, false)" alt="founder" class="w-100" v-show="index == 0">
                    </div>
                </div>
                <div class="col-5 my_cardRx">
                    <div class="my_description w-100 py-5 px-5">
                        <h2>
                            Jason Bickford
                        </h2>
                        <p class="text-secondary">
                            Founder and Executive Director
                        </p>
                        <div class="my_separator"></div>
                        <p class="text-body-tertiary">
                            Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas possimus, ut nemo fugit
                            vero quas...
                        </p>
                        <div class="row justify-content-between">
                            <div class="col">
                                <a class="my_socialIcon">
                                    <i class="fa-brands fa-linkedin-in"></i>
                                </a>
                                <a class="my_socialIcon">
                                    <i class="fa-brands fa-facebook-f"></i>
                                </a>
                                <a class="my_socialIcon">
                                    <i class="fa-brands fa-twitter"></i>
                                </a>
                            </div>
                            <div class="col">
                                <!-- spazio per eventuale firma -->
                            </div>
                        </div>

                    </div>
                </div>
            </div>

            <div class="my_bkgCircle position-absolute">
                <img src="../../assets/svg/svg-4.svg" class="">
            </div>
        </div>

    </div>
</template>

<style scoped>
.my_socialIcon {
    text-decoration: none;
    color: white;

}

.my_socialIcon i {
    background-color: rgb(255, 70, 18);
    padding: 0.4rem;
    font-size: 1rem;
    height: 1.8rem;
    width: 1.8rem;
    border-radius: 50%;
    text-align: center;
    margin-right: 1rem;
}

p {
    margin-top: 1rem;
}

.my_container {
    max-width: 2000px;
    position: relative;
    margin: 0 auto;
    z-index: 0;
}

.my_cardLx {
    margin-right: -2rem;
}

.my_cardRx {
    margin-left: -2rem;
}

.bkg_fafafa {
    background-color: #FAFAFA;
    color: black;
    width: 100%;
}

.my_description {
    background-color: #FFFFFF;
}

.my_separator {
    border: solid 0.08rem #FF4612;
    width: 5rem;
}

.my_bkgCircle {
    top: -3rem;
    right: 0;
    width: 30%;
    max-width: 30rem;
    z-index: -1;
    margin-right: 2rem;
}

.my_bkgCircle>img {
    object-fit: cover;
    max-width: 100%;
}
</style>