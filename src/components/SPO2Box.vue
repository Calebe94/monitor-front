<template>  
        <div class="card-small blue-grey darken-3">
            <div class="card-content white-text">
                <span class="card-title">SPO2</span>
                <h3 class="card-title" style="color: #ffea00"> {{ porcentage }} %</h3> 
                <div class="progress" style="padding: 10px">
                    <div class="determinate" style="width: 80%"></div>
                </div>
            </div>
        </div>
    <!-- </div> -->
</template>
<script src="js/kendo.all.min.js"></script>
<script>

    export default {
        name: 'SPO2Box',
        props: {
            porcentage: String
        }
    }

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    @import "~materialize-css/dist/css/materialize.css";

</style>
