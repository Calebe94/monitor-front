<template>
    <div class="col">
        <div class="row">
            <div class="card-panel blue-grey darken-3">
                <div class="card-content">
                    <SPO2Chart/>
                </div>    
            </div>
        </div>
        <div class="row">
            <div class="card-panel blue-grey darken-3">
                <div class="card-content">
                    <NIBPChart />
                </div>    
            </div>    
        </div>
        <div class="row">
            <div class="card-panel blue-grey darken-3">
                <div class="card-content">
                    <HRChart />
                </div>    
            </div>
        </div>
    </div>
</template>

<script>
    import SPO2Chart from '@/components/SPO2Chart.vue'
    import NIBPChart from '@/components/NIBPChart.vue'
    import HRChart from '@/components/HRChart.vue'


    export default {
        name: "ColumnCharts",
        components: {
            SPO2Chart,
            NIBPChart,
            HRChart
        }
    }
</script>
