<script>
import MyAppHeader from './components/MyAppHeader.vue';
import MyAppMain from './components/MyAppMain.vue';
import MyAppFooter from './components/MyAppFooter.vue';
import store from "./data/store.js"
export default{
  components:{
    MyAppFooter,
    MyAppHeader,
    MyAppMain
  },
  data(){
    return{
      store,
      percorso : "./assets/img/"
    }
  },
  methods:{
  },
  mounted(){
    console.log(`${this.percorso} `)
  }
}
</script>

<template>
  <img :src="this.percorso + store.immagini.jumbotron[0]" alt="">
  <MyAppHeader />
  <MyAppMain />
  <MyAppFooter />
</template>

<style scoped>
</style>
