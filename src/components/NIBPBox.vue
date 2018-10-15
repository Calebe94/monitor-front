<template>  
    <!-- <div class="col s3 m3 l3"> -->
        <div class="card-small blue-grey darken-3">
            <div class="card-content white-text">
                <span class="card-title">NIBP</span>
                <h3 class="card-title" style="padding:10px"> {{ systolic }} / {{ diastolic }} ({{ mean_pressure }})</h3> 
            </div>
        </div>
    <!-- </div> -->
</template>
<script src="js/kendo.all.min.js"></script>
<script>

    export default {
        name: 'NIBPBox',
        props: {
            systolic: String,
            diastolic: String,
            mean_pressure: String
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
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
    .row .col.s4 {
        /* padding: 0; */
    }
</style>
