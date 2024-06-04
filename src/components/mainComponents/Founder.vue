<script>
export default{
    name:"Founder",
    props:{
        foundersImg: Array
    },
    methods:{
        getSvg(name,isSvg) {
            if(isSvg){
                return new URL(`../../assets/svg/${name}`, import.meta.url).href;
            }else{
                return new URL(`../../assets/img/${name}`, import.meta.url).href;
            }
        }
    }
}
</script>

<template>
    <div class="bkg_fafafa py-5">
        <div class="row justify-content-center align-items-center g-0">
            <div class="col-4 my_cardLx">
                <div class="my_carousel w-100" v-for="element,index in foundersImg">
                    <img :src="getSvg(element,false)" alt="founder" class="w-100" v-show="index==0">
                </div>
            </div>
            <div class="col-4 my_cardRx">
                <div class="my_description w-100 py-5 px-4">
                    <h2>
                        Jason Bickford
                    </h2>
                    <p>
                        Founder and Executive Director
                    </p>
                    <div class="my_separator"></div>
                    <p>
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas possimus, ut nemo fugit vero quas...
                    </p>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.my_cardLx{
    margin-right:-2rem;
}
.my_cardRx{
    margin-left:-2rem;
}
.bkg_fafafa {
    background-color: #FAFAFA;
    color: black;
    width:100%;
}
.my_description{
    background-color: #FFFFFF;
}
.my_separator {
    border: solid 0.08rem #FF4612;
    width: 5rem;
}
</style>