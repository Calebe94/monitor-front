<template>
  <div class="home">
    <div class="container">
      <swiper :options="swiperOption">
        <swiper-slide>
          <link rel="stylesheet" 
            href="https://use.fontawesome.com/releases/v5.2.0/css/all.css" 
            integrity="sha384-hWVjflwFxL6sNzntih27bfxkr27PmbbK/iSvJ+a4+0owXq79v+lsFkW54bOGbiDQ" 
            crossorigin="anonymous">
          
          <!-- <div class="row">
            <div class="col">
              <ColumnBoxes/>
            </div>
            <div class="col">
              <ColumnCharts/>
            </div>
          </div>   -->

          <div class="card-small blue-grey darken-3" >
            <div class="row">
              <div class="col s4 m4 l4">
                <div class="card-content">
                  <SPO2Box porcentage="80"/>
                </div>
              </div>
              <div class="col s8 m8 l8">
                <div class="card-content">
                  <SPO2Chart/>
                </div>
              </div>
            </div>
          </div>

          <div class="card-small blue-grey darken-3">
            <div class="row">
              <div class="col s4 m4 l4">
                <div class="card-content">
                  <NIBPBox systolic="129" diastolic="87" mean_pressure="94" />
                    </div>
                  </div>
                <div class="col s8 m8 l8">
                  <div class="card-content">
                    <NIBPChart />
                  </div>
                </div>
            </div>
          </div>

          <div class="card-small blue-grey darken-3">
            <div class="row">
              <div class="col s4 m4 l4">
                <div class="card-content">
                  <HRBox bpm="50" temp_type="C" temp="36.6"/>
                </div>
              </div>
              <div class="col s8 m8 l8">
                <div class="card-content">
                  <HRChart />
                </div>
              </div>
            </div>
          </div>

        </swiper-slide>

        <swiper-slide>
          <!-- <Config/> -->
          <div class="container">
            <PatientInfoBox/>
          </div>
        </swiper-slide>
      </swiper>

      <FooterMenu/>
    </div>
    
    <div class="swiper-pagination"  slot="pagination"></div>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
import SPO2Box from '@/components/SPO2Box.vue'
import SPO2Chart from '@/components/SPO2Chart.vue'

import NIBPBox from '@/components/NIBPBox.vue'
import NIBPChart from '@/components/NIBPChart.vue'

import HRBox from '@/components/HRBox.vue'
import HRChart from '@/components/HRChart.vue'

import PatientInfoBox from '@/components/PatientInfoBox.vue'
import FooterMenu from '@/components/FooterMenu.vue'

import ColumnCharts from '@/components/ColumnCharts.vue'
import ColumnBoxes from '@/components/ColumnBoxes.vue'

/* SWIPER */
import 'swiper/dist/css/swiper.css'
import { swiper, swiperSlide } from 'vue-awesome-swiper'
import Config from '@/views/Config.vue';

export default {
  name: 'home',
  components: {
    // HelloWorld,
    SPO2Box,
    SPO2Chart,
    NIBPBox,
    NIBPChart,
    HRBox,
    HRChart,
    swiper, 
    swiperSlide,
    Config,
    PatientInfoBox,
    FooterMenu,
    ColumnCharts,
    ColumnBoxes,
  }
}
</script>

<style scoped>

</style>
