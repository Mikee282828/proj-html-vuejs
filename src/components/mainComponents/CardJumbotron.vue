<script>
export default {
    name: "CardJumbotron",
    data() {
        return {

        }
    }
}
</script>

<template>
    
    <div>
        <h1>OUR TEAM</h1>
        <p style="width: 50%;">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Rem at perferendis
            culpa pariatur aperiam
            corrupti blanditiis, fugit dolo.</p>
        <a href="#" class="btn btn-white btn-lg bg-white me-3 p-3" data-mdb-ripple-init role="button"
            aria-pressed="true">READ MORE <span class="lineVertical "></span> <span class="arrow ms-2">⟶</span></a>
        <a href="#" class="orange btn btn-lg p-3 text-white" data-mdb-ripple-init role="button"
            aria-pressed="true">PURCHASE <span class="lineVertical"></span> <span class="arrow ms-2">⟶</span></a>
    </div>
    
</template>

<style scoped>
.lineVertical {
    margin-left: 2rem;
    height: 100%;
    border-left: 1px solid;
}

.orange {
    background-color: #FF4612;
}




</style>