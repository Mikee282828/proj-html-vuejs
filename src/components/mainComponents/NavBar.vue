<script>

export default {
    name: "NavBar",
    data() {
        return {

        }
    }
}
</script>

<template>
    <nav class="navbar navbar-light bg-trasparent p-5">
        <div class="containerNav d-flex">
            <!-- LOGO NAV -->
            <div>
                <a class="navbar-brand" href="#">
                    <img src="../../assets/img/logo-img-01.png" width="25" height="25" class="logoHeader align-top">

                </a>
            </div>

            <!-- DROPDOWN LINK NAV -->
            <div class="dropdown d-flex">


                <div class="text-dark">⟶</div>
                <div class="dropdown">
                    <a class="dropdown-item pe-4 text-dark fw-bold" href="#" id="dropdownHomes"
                        data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                        HOMES
                    </a>

                    <div class="dropdown-menu" aria-labelledby="dropdownHomes">
                        <a class="dropdown-item" href="#">Action</a>
                        <a class="dropdown-item" href="#">Another action</a>
                        <a class="dropdown-item" href="#">Something else here</a>
                    </div>
                </div>


                <div class="text-dark">⟶</div>
                <div class="dropdown">
                    <a class="dropdown-item pe-4 text-dark fw-bold" href="#" id="dropdownHomes"
                        data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                        HOMES
                    </a>

                    <div class="dropdown-menu" aria-labelledby="dropdownHomes">
                        <a class="dropdown-item" href="#">Action</a>
                        <a class="dropdown-item" href="#">Another action</a>
                        <a class="dropdown-item" href="#">Something else here</a>
                    </div>
                </div>


                <div class="text-dark">⟶</div>
                <div class="dropdown">
                    <a class="dropdown-item pe-4 text-dark fw-bold" href="#" id="dropdownHomes"
                        data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                        HOMES
                    </a>

                    <div class="dropdown-menu" aria-labelledby="dropdownHomes">
                        <a class="dropdown-item" href="#">Action</a>
                        <a class="dropdown-item" href="#">Another action</a>
                        <a class="dropdown-item" href="#">Something else here</a>
                    </div>
                </div>

                <div class="text-dark">⟶</div>
                <div class="dropdown">

                    <a class="dropdown-item pe-4 text-dark fw-bold" href="#" id="dropdownHomes"
                        data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                        HOMES
                    </a>

                    <div class="dropdown-menu" aria-labelledby="dropdownHomes">
                        <a class="dropdown-item" href="#">Action</a>
                        <a class="dropdown-item" href="#">Another action</a>
                        <a class="dropdown-item" href="#">Something else here</a>
                    </div>
                </div>

                <div class="text-dark">⟶</div>
                <div class="dropdown">

                    <a class="dropdown-item pe-4 text-dark fw-bold" href="#" id="dropdownHomes"
                        data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                        HOMES
                    </a>

                    <div class="dropdown-menu" aria-labelledby="dropdownHomes">
                        <a class="dropdown-item" href="#">Action</a>
                        <a class="dropdown-item" href="#">Another action</a>
                        <a class="dropdown-item" href="#">Something else here</a>
                    </div>
                </div>

                <div class="text-dark arrow">⟶</div>
                <div class="dropdown">

                    <a class="dropdown-item pe-4 text-dark fw-bold" href="#" id="dropdownHomes"
                        data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                        HOMES
                    </a>

                    <div class="dropdown-menu" aria-labelledby="dropdownHomes">
                        <a class="dropdown-item" href="#">Action</a>
                        <a class="dropdown-item" href="#">Another action</a>
                        <a class="dropdown-item" href="#">Something else here</a>
                    </div>
                </div>

                <a class="dropdown-item pe-4 text-dark fw-bold" href="#">
                    <i class="fa-solid fa-magnifying-glass"></i>
                </a>

                <a class="dropdown-item pe-3 text-dark fw-bold" href="#">
                    <i class="fa-solid fa-bars"></i>
                </a>

            </div>

        </div>
    </nav>
</template>

<style scoped>
.containerNav {
    margin-left: 2rem;
    width: 100%;
    justify-content: space-between;
    flex-wrap: inherit;
    align-items: center;
}

.logoHeader {
    width: 100%;

}
</style>