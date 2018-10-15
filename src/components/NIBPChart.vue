<template>
    <div class="card-small blue-grey darken-2">
            <!-- <apexcharts width="60%" type="line" :options="chartOptions" :series="series"></apexcharts> -->
        <trend  
            :data="[5, 2, 5, 9, 5, 10, 3, 5, 0, 0, 1, 8, 2, 9, 0]"
            :gradient="['#6fa8dc', '#42b983', '#2c3e50']"
            auto-draw
            smooth>
        </trend>
    </div>
</template>

<script>

    import Vue from 'vue';
    import VueApexCharts from 'vue-apexcharts'
    import Trend from 'vuetrend';

    Vue.use(Trend);

    export default {
        components: {
        apexcharts: VueApexCharts,
        },
        data: function() {
            return {
                chartOptions: {
                    chart: {
                        id: 'vuechart-example'
                    },
                    xaxis: {
                        categories: [1991, 1992, 1993, 1994, 1995, 1996, 1997, 1998]
                    }
                },
                series: [{
                    name: 'series-1',
                    data: [30, 40, 45, 50, 49, 60, 70, 91]
                }]
            }
        },
    };
</script>
<style scoped>
    @import "~materialize-css/dist/css/materialize.css";
    
    /* h3 {
    margin: 40px 0 0;
    }
    ul {
    list-style-type: none;
    padding: 0;
    }
    li {
    display: inline-block;
    margin: 0 10px;
    }
    a {
    color: #42b983;
    } */
    .row .col.s8 {
        /* padding: 0; */
    }
</style>

