<template>
  <div class="aboutusmain animated ">
    <div class="mainbox">
      <parallax :speed-factor="0">
        <!-- <img src="/img/carcrop2.jpg"> -->
        <v-carousel>
            <v-carousel-item
              v-for="(item,i) in items"
              :key="i"
              :src="item.src"
            ></v-carousel-item>
          </v-carousel>

      </parallax>
        <div class="maincopy animated zoomInUp">
          <div class="boxone">
            <p class="electrify">ELECTRIFYING</p>
            <p class="yous"><span class="yoursmall">YOUR</span><span class="your"> JOURNEY</span></p>
          </div>
          <div class="boxtwo">
            <div class="titleblurb">
              <p class="blurb2">FIND YOUR CHARGING STATION</p>
            </div>
            <div class="pickbox">
              <div class="pickbox">
                <div class="firstpic">
                  <a href="https://na.chargepoint.com/charge_point" target="_blank">
                  <!--<img src="/img/chargepoint_logo.png">-->
                    <img src="/img/chargepoint_logo_small.png">
                  </a>
                </div>
                <div class="otherpic">
                  <a href=" https://flo.ca/on-the-go/map" target="_blank">
                    <img src="/img/flologo.png">
                  </a>
                </div>
              </div>
            </div>
          </div>
        </div>
    </div>


  <div class="aboutus">
    <div class="aboutbox" id="abus">
      <div class="innerbox2">
        <div class="abouttitlebox">
          <div class="aboutustext">
            ABOUT US
          </div>
        </div>
        <div class="aboutcopybox"><br><br>
          <p class="philosophy">Our Philosophy</p><br>
          <p class="blurb2">OZZ EV and with Weis & Associates Inc, two leading forces in electrification and infrastructure management have 
            partnered to bring full turn-key EV services for OEM & Dealer Clients in the Automotive Industry</p><br>
          <p class="blurb2">With a vision for a greener world, 
            OZZ EV is a key player in building a sustainable and practical network of EV charging stations nationwide.
            OZZ EV prides itself on its ability to provide full turnkey solutions that are efficient, of high quality and economical. 
            We aim to do this by leveraging our strengths, resources, technology and strategic partners to fulfill this complex project. 
            Let us electtrify your journey!</p><br>
          <br><br>
          <p class="blurb2">A division of Ozz Electric</p>
          <div class="aboutimg">
            <a href="http://www.ozzelectric.com/" target="_blank">
              <img src="/img/ozzelectric.png" alt="Logo">
            </a>
          </div>
        </div>
      </div>
      </div>
  </div>

    <!--<Aboutus />-->

  <div class="solutions" id="oursol">
    <div class="solhalf">
      <div class="solutionbox1">
        <div class="oursolution">OUR SOLUTIONS</div>
      </div>
      <div class="solutionbox2">
        <div class="workicon">
          <img src="/img/3building.png" alt="work"/>
            <div class="caption">
              <br>
              <p>WORK</p>
            </div>
        </div>
        <div class="familyicon">
          <img src="/img/4rent.png" alt="family"/>
            <div class="caption">
              <br>
              <p>FAMILY</p>
            </div>
        </div>
        <div class="cityicon">
          <img src="/img/1town.png" alt="city"/>
            <div class="caption">
              <br>
              <p>CITY</p>
            </div>
        </div>
        <div class="retailicon">
          <img src="/img/2retail.png" alt="retail"/>
            <div class="caption">
              <br>
              <p>RETAIL</p>
            </div>
        </div>
      </div>


      <div class="solutionbox3">
        <p class="innersolutiontexttitle">EV Charging Diversity</p>
        <p class="innersolutiontext">OZZ EV Solutions sources charging stations from all major manufacturers.</p>
        <p class="innersolutiontext">By working with all major manufacturers, we understand the unique features of each charging station.</p>
      </div>
      <div class="solutionbox4">
        <p class="innersolutiontexttitle">Our Mission: EV Charging, Everywhere</p>
        <p class="innersolutiontext">Convenient and connected charging for home, work, around town and out of town.</p>
      </div>
      <div class="solutionbox5">
        <div class="weisboxone">
          <p class="innersolutiontexttitle">Support Powered by WE!S</p>
          <p class="innersolutiontext">Weis provides valuable software, project management and consulting support to OZZ ev solutions in particular with the automotive industry where they have strong Customer Experience and Dealership Process knowledge.</p>
        </div>
          <div class="weisboxtwo">
            <a href="https://www.weis.ca/" target="_blank">
              <img class="aboutimg" src="/img/weislogo1.png">
            </a>
          </div>

      </div>
    </div>
  </div>

    <div class="newsevenstep">
      <div class="newsevencopy">
        <p class="innersolutiontexttitle">3 Easy Steps to EV Charging</p>-->
        <br>
        <p class="innersolutiontext">Step 1 - Customer can either book pre-inspection online or book installation at participating Car Dealerships following your vehicle purchase.</p>
        <br>
        <p class="innersolutiontext">Step 2 - A work order for installation is created and an OZZ ev Technician is notified to visit your home, office or other. We are a nationwide company able to install almost anywhere in Canada.</p>
        <br>
        <p class="innersolutiontext">Step 3 - An OZZ ev Installation technician is confirmed and date is agreed to complete the installation.</p>
        <br>
        <br>
      </div>
    </div>

    <div class="productcare">
      <div class="carou">
        <no-ssr>
          <carousel :items="1" :center="true" :nav="false" :loop="true" :autoplay="true">

            <div class="itembox">
              <div class="itemimage">
                <img src="/img/250DC.jpg" alt="250DC.jpg">
              </div>
              <div class="itemcopy">
                <p class="itemtitle">Express 250 DC Fast Charging Stations</p>
                <br>
                <p>Express 250 stations are ideal for businesses near major roads where drivers need quick turnaround charging.</p>
                <p>Express stations can also complement CT4000 stations at workplaces, offering employees a quick charge when they need it.</p>
              </div>
            </div>

            <div class="itembox">
              <div class="itemimage">
                <img src="/img/flo_coreplsu_wallmount.png" alt="250DC.jpg">
              </div>
              <div class="itemcopy">
                <p class="itemtitle">CORE+</p>
                <p class="itemtitle">PEDESTAL SINGLE</p>
                <br>
                <p>CoRe+ charging stations are perfectly adapted for a wide range of parking environments including workplaces, multi-unit residential buildings and commercial properties. They are ideal for areas where many electric vehicles need to charge simultaneously, as they can be cascaded to minimize installation costs for the entire site.</p>
                <br>
              </div>
            </div>

          </carousel>
        </no-ssr>
      </div>
    </div>
  </div>
</template>

<script>
import carousel from 'vue-owl-carousel'
import Parallax from 'vue-parallaxy'
import VShowSlide from 'v-show-slide'

import Aboutus from "~/components/Aboutus.vue";

export default {

  components: {
    Aboutus
  },

  head: {
    meta: [
      { charset: 'utf-8'},

    ]
  },

  data () {
    return {
      items: [
        {
          src: require('./../assets/slider/slider1.png'),
        },{
          src: require('../assets/slider/slider2.png'),
        },{
          src: require('../assets/slider/slider3.png'),
        },{
          src: require('../assets/slider/slider4.png'),
        },{
          src: require('../assets/slider/slider5.png'),
        },{
          src: require('../assets/slider/slider6.png'),
        },
      ],
    }
  },
  components: { carousel, Parallax }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.aboutusmain {
  grid-column :1/7;
  grid-row: 2 / 3;
  animation-duration: 5s;
}


</style>
