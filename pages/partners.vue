<template>
  <div class="wholebox">
    <div class="partners" id="partone">
    <!--<parallax :speed-factor="0.3">-->
      <!--<img src="/img/partback.jpg">-->
    <!--</parallax>-->
    <div class="partnerbox">
      <p class="partnertitle">PARTNERS</p>
      <img src="/img/flologo.png">
      <br>
      <div class="partnercopy firstpart">We partner with FLO, Canada's leading electronic vehicle (EV) charging station network. Together, OZZ ev solutions and FLO provide clean, sustainable solutions for cities and municipalities, commercial real estate properties, multi-unit residential buildings, retail stores and restaurants, and corporate organizations.</div>
      <br>
      <p class="partnersubtitle">WHO IS FLO?</p>
      <div class="parntercopy secondpart">FLO operates Canada's largest EV charging network and the second largest in North America. For close to a decade*, we have built a reputation on quality and reliability that has defined us as an industry leader in the development of EV infrastructure in Canada and the US, and a preferred choice for utilities, cities, employers and EV drivers.</div>
      <p class="appen">*FLO is a subsidiary company of AddEnergie</p>
      <br>
      <p class="partnersubtitle">Customizable solutions for all types of properties</p>
      <p>No matter what your requirements are, we offer flexible and affordable solutions for any situation.</p>
      <br>
      <div class="choices">
        <div class="choice1">
          <p class="bluesub bluetitle">Parking areas with assigned spaces</p>
          <p class="partnercopy">Allow residents to have a dedicated charging station at their assigned parking space with no impact on other occupants.</p>
          <br>
          <br>
          <p class="partnersubtitle bold">WHY CHOOSE FLO?</p>
          <p class="bold">FLO is Canada's largest electric vehicle charging network.</p>
          <p>We operate <span class="bold">thousands</span> of charging stations from coast to coast, with an <span class="bold">industry-leading</span> reliability rate.</p>
          <ul class="bluetitle">
            <li>Turnkey, flexible solutions for all types of properties</li>
            <li>Real-time charging station monitoring</li>
            <li>Remote servicing and troubleshooting</li>
            <li>Simple pricing and access control</li>
            <li>Detailed data reports accessible at all times</li>
            <li>24/7 bilingual support line for EV drivers</li>
            <li>Scalable solutions to meet current and future demand</li>
            <li>Connection with more than 80% of Canadian EV drivers</li>
          </ul>

        </div>
        <div class="choice2">
          <div class="topchoice2">
            <p class="bluesub bluetitle">Shared parking spaces</p>
            <p class="partnercopy">Offer shared charging stations to residents-free of charge or for a fee-in your building's common parking area.</p>
          </div>
          <div class="bottomchoice2">
            <p class="partnersubtitle">DID YOU KNOW?</p>
            <p>On average, between 60 and 80% of EV charging is done at home.</p>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="partners2" id="parttwo">
    <div class="chargebox">
      <img src="/img/chargepoint_logo.png" alt="smarttwo"/>
    </div>
    <div class="chargecopy">
      <p>OZZ ev solutions  partner with Charge Point, that brings electric vehicle (EV) charging to more people and places than ever before.</p>

      <p>ChargePoint operates the world’s largest and most open EV charging network. We also design, build, and support the technology that powers it. As our network grows, it makes driving an EV accessible to more and more people.</p>

      <p>Together our mission is to get everyone behind the wheel of an EV and provide a place for them to charge wherever they go.  We’re transforming the transportation industry by providing the charging stations, mobile app, and the network that allow people to charge their cars everywhere they go.</p>

    </div>

    <div class="productcare">
      <carousel class="productbox" :autoplay="true" :nav="false" :number="1" :center="true" :autoHeight="true" :autoWidth="true" >
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

      </carousel>

    </div>

  </div>

  </div>
</template>
<script>
  import Parallax from 'vue-parallaxy'

  export default {
    components: { Parallax}
  }
</script>

<style>
  .partners img {
    /*width: 100vw;*/
    /*transform: scale(1.5,1.5) scaleX(-1) ;*/
    /*padding: 2%;*/
  }
  .Masthead {
    grid-row: 1/2;
  }

</style>
