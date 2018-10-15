<template>
    <!-- <div class="col s9 m9 l9"> -->
        <div class="card-small blue-grey darken-2">
            <!-- <apexcharts width="60%" type="line" :options="chartOptions" :series="series"></apexcharts> -->
            <trend 

                :data="[0, 1, 2, 1, 2, -5, 9, 0, 1, 4, 2, 1, 0, 0, 0, 0, 0, 1, 2, 1, 2, -5, 9, 0, 1, 4, 2, 1, 0, 0, 0, 0, 0, 1, 2, 1, 2, -5, 9, 0, 1, 4, 2, 1, 0, 0, 0, 0, 0, 1, 2, 1, 2, -5, 9, 0, 1, 4, 2, 1, 0, 0, 0, 0, 0, 1, 2, 1, 2, -5, 9, 0, 1, 4, 2, 1, 0, 0, 0, 0, 0, 1, 2, 1, 2, -5, 9, 0, 1, 4, 2, 1, 0, 0, 0, 0, 0, 1, 2, 1, 2, -5, 9, 0, 1, 4, 2, 1, 0, 0, 0, 0, 0, 1, 2, 1, 2, -5, 9, 0, 1, 4, 2, 1, 0, 0, 0, 0, ]"
                :gradient="['#6fa8dc', '#42b983', '#2c3e50']"
                auto-draw
                >
            </trend>
        </div>
    <!-- </div> -->
</template>

<script>

    import Vue from 'vue';
    // import VueApexCharts from 'vue-apexcharts'
    import Trend from 'vuetrend';

    Vue.use(Trend);
    
    export default{
        name: "HRChart"

    }

</script>
<style scoped>
    @import "~materialize-css/dist/css/materialize.css";
    
</style>

