<template>
  <div class="wholebox">
    <div class="partners" id="partone">
      <div class="partnerbox">
        <p class="partnertitle">General Information</p>
        <br>
        <p class="partnersubtitle">What is EV Home Charging</p>
        <div class="partnercopy firstpart">All electric cars need to be charged by plugging in. You can recharge using a standard wall socket or an EV charging station. The time it takes to fully charge is based on the level, or speed, of charging and how full the battery is.</div>
        <br>
        <p class="partnersubtitle">Charge Using a Regular Wall Socket (Level 1)</p>
        <p class="partnersubtitle"> 1 Hour of Charging ~ 8 km of Driving Range  </p>
        <br>
        <div class="partnercopy firstpart">All EV models come standard with a portable cord-set that lets you charge using any standard household outlet. This is called Level 1 charging and is the slowest speed of charging, but ensures that no matter where you are, you can always recharge.
   If you are driving a plug-in hybrid, it is possible that Level 1 charging is all you really need. Level 1 will fully recharge most plug-in hybrids on the market over-night.
        </div>
        <br>
        <p class="partnersubtitle">Charge Using an EV Charging Station (Level 2)</p>
        <p class="partnersubtitle">1 Hour of Charging ~ 30 km of Driving Range </p>

        <div class="parntercopy secondpart">The Best Time to Charge is at Night when the Cost of Electricity is Lowest Many jurisdictions offer "peak-pricing" on electricity. 
          This means that electricity is more expensive during the day when the demand is highest and less expensive during the night when the demand is lowest. 
          This is excellent news for EV drivers because during the night is also the most convenient time to charge. 
          Get home, plug-in and wake-up to a full battery of low-cost electricity.</div>
        <br>
      </div>
    </div>
    <div class="partners2" id="parttwo">
      <div class="chargecopy">
        <p class="partnersubtitle">How do you install a Home Charging Station?</p>
        <p>A charging station installation is a complex process that requires a professional electrician. Here are some common items to be mindful of:</p>

        <p><strong>Electrical Service:</strong> Charging stations operate at 240 Volts and 30 Amps, which is similar to a clothes dryer or stove. Many homes, especially in older neighbourhoods, were not designed to accommodate the additional demand of a charging station and it is possible that your electrician will need to upgrade your electrical service.</p>

        <p><strong>Location:</strong> Most charging stations come with either a 20 ft. or 25 ft. cord. Make sure that the cord will reach from the charging station to your car’s charger port.</p>

        <p><strong>Plug-in Stations:</strong> These stations connect to a dryer plug (also known as a NEMA outlet). Every charging station requires a specific type of NEMA outlet. It is imperative that the NEMA outlet installed in your wall is compatible with the NEMA outlet used by your charging station.</p>

        <p class="partnersubtitle">Installing a Level 1 electric vehicle charger</p>
        <p>Level 1 EV chargers come with your electric vehicle and don’t require any special installation – 
          simply plug your Level 1 charger into a standard 120 volt wall outlet and you’re ready to go. 
          This is the biggest appeal of a Level 1 charging system: you don’t have to deal with any extra costs associated with an installation, 
          and you can set the entire charging system up without a professional.</p>
        <p class="partnersubtitle">Installing a Level 2 electric vehicle charger, the specifics.</p>
        <p>A level 2 EV charger uses 240 volts of electricity. 
          This has the benefit of offering faster charging time, but it requires a special installation procedure as a standard wall outlet only provides 120 volts. 
          Appliances like electric dryers or ovens use 240 volts as well, and the installation process is very similar.</p>
        <p class="partnersubtitle">Level 2 EV charger: The Specifics</p>
        <p>Level 2 installation requires running 240 volts from your breaker panel to your charging location. 
          A “double-pole” circuit breaker needs to be attached to two 120 volt buses at once to double the circuit voltage to 240 volts, 
          using a 4-strand cable. From a wiring perspective, this involves attaching a ground wire to the ground bus bar, 
          a common wire to the wire bus bar, and two hot wires to the double-pole breaker. 
          You may have to replace your breaker box entirely to have a compatible interface, 
          or you may be able to simply install a double-pole breaker in your existing panel. 
          It is essential to make sure that you shut off all power going into your breaker box by shutting off all breakers, 
          followed by shutting off your main breaker.</p>
        <p>Once you have the correct circuit breaker attached to your home wiring, 
          you can run your newly installed 4-strand cable to your charging location. 
          This 4-strand cable needs to be properly insulated and secured to prevent from damage to your electrical systems, 
          especially if it is being installed outdoors at any point. 
          The last step is to mount your charging unit where you will be charging your vehicle, 
          and attach it to the 240 volt cable. The charging unit acts as a safe holding location for the charge current, 
          and doesn’t let electricity flow through until it senses that your charger is connected to your car’s charging port.</p>
        <p>Considering the technical nature and risk of a Level 2 EV charger DIY installation, 
          it is always smart to hire a professional electrician to install your charging station. 
          Local building codes often require permits and inspections by a professional anyways, 
          and making an error with an electrical installation can cause cause material damage to your home and electrical systems.</p>
        <p>Electric work is also a health hazard, and it is always safer to let an experienced professional handle electric work.</p>

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
  .Masthead {
    grid-row: 1/2;
  }

</style>
