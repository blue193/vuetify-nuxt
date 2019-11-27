<template>
  <v-app>
    <v-menu
      offset-y
      content-class="dropmenu"
      transition="slide-y-transition">
      <v-btn
        slot="activator"
        color="white"
        icon>
        <v-icon>menu</v-icon>
      </v-btn>
      <v-card>
        <v-list dense>
          <div class="menubar">
            <nuxt-link to="/#abus"><v-list-tile-title>About Us</v-list-tile-title></nuxt-link>
            <nuxt-link to="/#oursol"><v-list-tile-title>Our Solutions</v-list-tile-title></nuxt-link>
              <v-menu offset-x
                      left open-on-hover>
                <v-list-tile slot="activator" >
                  <v-list-tile-action>
                  <!--<v-icon>play_arrow</v-icon>-->
                    <v-list-tile-title>Products</v-list-tile-title>
                  </v-list-tile-action>
                </v-list-tile>
                <v-list dense>
                  <div class="menubar">
                    <nuxt-link to="/products/chargepoint"><v-list-tile-title>ChargePoint</v-list-tile-title></nuxt-link>
                    <nuxt-link to="/products/flo"><v-list-tile-title>FLO</v-list-tile-title></nuxt-link>
                  </div>
                </v-list>
              </v-menu>
            <nuxt-link to="/incentives"><v-list-tile-title>Incentives</v-list-tile-title></nuxt-link>
              <v-menu offset-x left open-on-hover>
                <v-list-tile slot="activator" >
                  <v-list-tile-action>
                  <!--<v-icon>play_arrow</v-icon>-->
                    <v-list-tile-title>Partners</v-list-tile-title>
                  </v-list-tile-action>
                </v-list-tile>
                <v-list dense>
                  <div class="menubar">
                    <nuxt-link to="/partners#parttwo"><v-list-tile-title>ChargePoint</v-list-tile-title></nuxt-link>
                    <nuxt-link to="/partners#partone"><v-list-tile-title>FLO</v-list-tile-title></nuxt-link>
                  </div>
                </v-list>
              </v-menu>
          </div>
        </v-list>
      </v-card>
    </v-menu>
  </v-app>
</template>
