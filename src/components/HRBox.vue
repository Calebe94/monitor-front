<template>  
    <div class="card-small blue-grey darken-3">
        <div class="card-content white-text">
            <span class="card-title">HR(BPM)</span>
            <h4 class="card-title"> {{ bpm }} BPM</h4> 
            <div class="card blue-grey darken-3">
                <span class="card-title">Temp: {{ temp }} ˚{{ temp_type }} </span>
            </div>
        </div>
    </div>
</template>
<script src="js/kendo.all.min.js"></script>
<script>

    export default {
        name: 'HRBox',
        props: {
            bpm: String,
            temp: String,
            temp_type: String
        }
    }

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    @import "~materialize-css/dist/css/materialize.css";

</style>
