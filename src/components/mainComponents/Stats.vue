<script>
export default {
    data() {
        return {
            mentorship: 0,
            education: 0,
            learning: 0,
            motivation: 0,
            timer1: null,
            timer2: null,
            timer3: null,
            timer4: null,
        }
    },
    methods: {
        toPercentage() {
            this.timer1 = setInterval(() => {
                if (this.mentorship < 78) {
                    this.mentorship++;
                } else if (this.mentorship == 78) {
                    clearInterval(this.timer1)
                }
            }, 2000 / 78);

            this.timer2 = setInterval(() => {
                if (this.education < 95) {
                    this.education++;
                } else if (this.mentorship == 95) {
                    clearInterval(this.timer2)
                }
            }, 2000 / 95);

            this.timer3 = setInterval(() => {
                if (this.learning < 65) {
                    this.learning++;
                } else if (this.mentorship == 65) {
                    clearInterval(this.timer3)
                }
            }, 2000 / 65);

            this.timer4 = setInterval(() => {
                if (this.motivation < 83) {
                    this.motivation++;
                } else if (this.mentorship == 83) {
                    clearInterval(this.timer4)
                }
            }, 2000 / 83);
        }
    },
    mounted() {
        this.toPercentage();
    }
}
</script>

<template>
    <div class="row justify-content-center">
        <div class="col-5">
            <div class="my_title pb-5">
                <h2 class="">Creative Leader<span class="my_textOrange">.</span></h2>
                <div class="my_separator my-3"></div>
                <p class="text-body-tertiary">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quam quos
                    sapiente alias sed ipsam eveniet totam repellat. Officiis quibusdam, voluptates laboriosam odio fuga
                    animi sed alias maiores nihil magnam cupiditate!</p>
                <p><strong>READ MORE</strong></p>
            </div>
        </div>
        <div class="col-5">
            <div class="my_stat">
                <div class="my_statText d-flex justify-content-between">
                    <h5>Mentorship</h5>
                    <h5>{{ mentorship }}%</h5>
                </div>
                <div class="my_statBar">
                    <div class="my_statBarBase my_stat78"></div>
                </div>
            </div>

            <div class="my_stat">
                <div class="my_statText d-flex justify-content-between">
                    <h5>Education</h5>
                    <h5>{{ education }}%</h5>
                </div>
                <div class="my_statBar">
                    <div class="my_statBarBase my_stat95"></div>
                </div>
            </div>

            <div class="my_stat">
                <div class="my_statText d-flex justify-content-between">
                    <h5>Learning</h5>
                    <h5>{{ learning }}%</h5>
                </div>
                <div class="my_statBar">
                    <div class="my_statBarBase my_stat65"></div>
                </div>
            </div>

            <div class="my_stat">
                <div class="my_statText d-flex justify-content-between">
                    <h5>Motivation</h5>
                    <h5>{{ motivation }}%</h5>
                </div>
                <div class="my_statBar">
                    <div class="my_statBarBase my_stat83"></div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.row {
    background-color: #FAFAFA;
    color: black;
}

.my_separator {
    border: solid 0.08rem #FF4612;
    width: 5rem;
}

.my_textOrange {
    color: #FF4612;
}

.my_stat {
    margin-bottom: 2rem;
}

.my_statBar {
    width: 100%;
    border-bottom: solid rgba(0, 0, 0, 0.223) 1px;
    position: relative;
}

.row {
    max-width: 1400px;
    margin: 0 auto;
    padding: 7rem;
}

.my_statBarBase {
    height: 3px;
    animation-duration: 2s;
    background-color: #FF4612;
}

.my_stat78 {
    width: 78%;
    animation-name: statBar78;
}

.my_stat95 {
    width: 95%;
    animation-name: statBar95;
}

.my_stat65 {
    width: 65%;
    animation-name: statBar65;
}

.my_stat83 {
    width: 83%;
    animation-name: statBar83;
}

@keyframes statBar78 {
    from {
        width: 0%;
    }

    to {
        width: 78%;
    }
}

@keyframes statBar95 {
    from {
        width: 0%;
    }

    to {
        width: 95%;
    }
}

@keyframes statBar65 {
    from {
        width: 0%;
    }

    to {
        width: 65%;
    }
}

@keyframes statBar83 {
    from {
        width: 0%;
    }

    to {
        width: 83%;
    }
}
</style>