<template>
    <div class="card-small blue-grey darken-3">
        <div class="row">
            <div class="col s2 m2 l2">
                <div class="card-content">
                    <div class="card-panel blue-grey darken-2">
                        <div class="card-content white-text">
                            <h4 class="card-name"> <i class="fas fa-volume-off"></i> </h4>
                            <h5 class="card-name"> Sound </h5>
                        </div>
                    </div>
                </div>
            </div>
            <div class="col s2 m2 l2">
                <div class="card-content">
                    <div class="card-panel blue-grey darken-2">
                        <div class="card-content white-text">
                            <h4 class="card-name"> <i class="fas fa-bell-slash"></i> </h4>
                            <h5 class="card-name"> Alarm </h5>
                        </div>
                    </div>
                </div>
            </div>
            <div class="col s2 m2 l2">
                <div class="card-content">
                    <div class="card-panel blue-grey darken-2">
                        <div class="card-content white-text">
                            <h4 class="card-name"> <i class="fas fa-chart-bar"></i> </h4>
                            <h5 class="card-name"> Stats </h5>
                        </div>
                    </div>
                </div>
            </div>
            <div class="col s2 m2 l2">
                <!-- <a href=""> -->
                <router-link to="/patient">
                <div class="card-content">
                    <div class="card-panel blue-grey darken-2">
                        <div class="card-content white-text">
                            <h4 class="card-name"> <i class="fas fa-user"></i> </h4>
                            <h5 class="card-name"> Patient </h5>
                        </div>
                    </div>
                </div>
                </router-link>
                <!-- </a> -->
            </div>
            <div class="col s2 m2 l2">
                <div class="card-content">
                    <div class="card-panel blue-grey darken-2">
                        <div class="card-content white-text">
                            <h4 class="card-name"> <i class="fas fa-chart-area"></i> </h4>
                            <h5 class="card-name"> Limits </h5>
                        </div>
                    </div>
                </div>
            </div>
            <div class="col s2 m2 l2">
                <div class="card-content">
                <router-link to="/config">
                    <div class="card-panel blue-grey darken-2">
                        <div class="card-content white-text">
                            <h4 class="card-name"> <i class="fas fa-cog"></i></h4>
                            <h5 class="card-name"> Settings </h5>
                        </div>
                    </div>
                </router-link>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "FooterMenu"
    }
</script>
