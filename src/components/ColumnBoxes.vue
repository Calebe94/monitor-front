<template>
    <div class="col">
        <div class="row">
            <div class="card-panel blue-grey darken-3">
                <div class="card-content">
                    <SPO2Box porcentage="80"/>
                </div>    
            </div>
        </div>
        <div class="row">
            <div class="card-panel blue-grey darken-3">
                <div class="card-content">
                    <NIBPBox systolic="129" diastolic="87" mean_pressure="94" />
                </div>    
            </div>
        </div>
        <div class="row">
            <div class="card-panel blue-grey darken-3">
                <div class="card-content">
                    <HRBox bpm="50" temp_type="C" temp="36.6"/>
                </div>    
            </div>
        </div>
    </div>
</template>
<script>

    import SPO2Box from '@/components/SPO2Box.vue'
    import NIBPBox from '@/components/NIBPBox.vue'
    import HRBox from '@/components/HRBox.vue'
    // import { Multipane, MultipaneResizer } from 'vue-multipane';

    export default {
        name: "ColumnBoxes",
        components: {
            // HelloWorld,
            SPO2Box,
            NIBPBox,
            HRBox,
            // MultiPane,
            // MultiPaneResizer
        }
    }
</script>
