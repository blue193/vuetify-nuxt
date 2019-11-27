<template>
  <v-app>
  <div class="ultimate">
  <header>
    <div class="headtitle">
        <nuxt-link to="/">
          <img src="/img/titlelogo.png" alt="Logo">
        </nuxt-link>
    </div>
    <div class="menusplit2">


      <v-menu
        offset-y
        content-class="dropmenu"
        transition="slide-y-transition"
        close-on-content-click>
        <v-btn
          slot="activator"
          color="white"
          icon>
          <v-icon>menu</v-icon>
        </v-btn>
        <v-card>
          <v-list dense>
            <div class="menubar">
              <!--<nuxt-link to="/#abus"><v-list-tile-title>About Us</v-list-tile-title></nuxt-link>-->
              <v-list-tile-title><a href="/#abus"><span data-hover="About Us" >About Us</span></a></v-list-tile-title>
              <v-list-tile-title><a href="/#oursol"><span data-hover="Our Solutions" >Our Solutions</span></a></v-list-tile-title>
              <v-list-tile-title>Products</v-list-tile-title>
              <nuxt-link to="/products/chargepoint"><v-list-tile-sub-title>ChargePoint</v-list-tile-sub-title></nuxt-link>
              <nuxt-link to="/products/flo"><v-list-tile-sub-title>FLO</v-list-tile-sub-title></nuxt-link>
              <nuxt-link to="/incentives"><v-list-tile-title>Incentives</v-list-tile-title></nuxt-link>
              <v-list-tile-title>Partners</v-list-tile-title>
              <nuxt-link to="/partners#parttwo"><v-list-tile-sub-title>ChargePoint</v-list-tile-sub-title></nuxt-link>
              <nuxt-link to="/partners#partone"><v-list-tile-sub-title>FLO</v-list-tile-sub-title></nuxt-link>
              <nuxt-link to="/contact"><v-list-tile-title>Contact Us</v-list-tile-title></nuxt-link>

            </div>
          </v-list>
        </v-card>
      </v-menu>
    </div>

    <div class="requestquoter">
      <v-dialog v-model="dialog" class="quote" persistent max-width="50%">

        <v-card-title slot="activator" dark v-on="on">REQUEST A QUOTE</v-card-title>
        <v-card>
          <v-card-title class="requesttitle">
            REQUEST A QUOTE
          </v-card-title>
          <div class="quoteform">
            <div class="content">
              <form name="request" method="POST" data-netlify="true">
                <input type="hidden" name="form-name" value="request"/>
                <p>
                  <input class="form-field" type="text" name="name" id="name" placeholder="NAME*"/>
                </p>

                <p>
                  <input class="form-field" type="email" name="email" id="email" placeholder="EMAIL*" />

                </p>

                <p>
                  <textarea class="form-field" name="message" id="message" placeholder="MESSAGE*"></textarea>
                </p>

                <v-card-actions>
                  <v-spacer></v-spacer>
                  <v-btn color="blue darken-1" type="submit" value="send message" flat @click="dialog = false">SUBMIT</v-btn>
                  <v-btn color="blue darken-1" flat @click="dialog = false">CLOSE</v-btn>
                </v-card-actions>
              </form>
            </div>
          </div>

        </v-card>


      </v-dialog>
    </div>
   
    <div class="menusplit">
      <div class="display-flex">
          <v-row class="justify-end">
              <v-btn color="transparent" class="ma-2" dark @click="bookAnInstall">
                BOOK AN INSTALL
              </v-btn>
              <v-btn
                color="transparent"
                class="ma-2"
                dark
                @click="dialog2 = true"
              >
                REQUEST A QUOTE
              </v-btn>
              <v-dialog v-model="dialog2" persistent max-width="50%">
                  <!-- <v-card-title slot="activator" dark v-on="on">REQUEST A QUOTE</v-card-title> -->
                    <v-card>
                      <v-card-title class="requesttitle">
                        REQUEST A QUOTE
                      </v-card-title>
                      <div class="quoteform">
                        <div class="content">
                          <form name="request" method="POST" data-netlify="true">
                            <input type="hidden" name="form-name" value="request"/>
                            <p>
                              <input class="form-field" type="text" name="name" id="name" placeholder="NAME*"/>
                            </p>
            
                            <p>
                              <input class="form-field" type="email" name="email" id="email" placeholder="EMAIL*" />
            
                            </p>
            
                            <!--<p>-->
                              <!--<input class="form-field" name="subject" id="subject" placeholder="SUBJECT" />-->
                            <!--</p>-->
            
                            <p>
                              <textarea class="form-field" name="message" id="message" placeholder="MESSAGE*"></textarea>
                            </p>
            
                            <!--<p><input class="form-button" type="submit" value="SEND MESSAGE" /></p>-->
                            <v-card-actions>
                              <v-spacer></v-spacer>
                              <v-btn color="blue darken-1" type="submit" value="send message" flat @click="dialog2 = false">SUBMIT</v-btn>
                              <v-btn color="blue darken-1" flat @click="dialog2 = false">CLOSE</v-btn>
                            </v-card-actions>
                          </form>
                        </div>
                      </div>
            
                    </v-card>
            
            
                  </v-dialog>
            </v-row>
      </div>
      
      <nav class="menubar">

          <ul class="cl-effect-5">
            <!--<li><nuxt-link to="/#abus" @click="$router.go{{path:'/#abus', force: true}}"><span data-hover="About Us" >About Us</span></nuxt-link></li>-->
            <!--<li><button @click="$router.go{path:'/#abus', force: true}"><span data-hover="About Us" >About Us</span></button></li>-->
            <li><a href="/#abus"><span data-hover="About Us" >About Us</span></a></li>
            <li><a href="/#oursol"><span data-hover="Our Solutions" >Our Solutions</span></a></li>
            <!--<li><nuxt-link to="/#oursol"><span data-hover="Our Solutions">Our Solutions</span></nuxt-link></li>-->

        <!--<li><nuxt-link to="/products"><span data-hover="Products">Products</span></nuxt-link></li>-->

            <li><v-menu open-on-hover allow-overflow auto offset-y>
              <v-text slot="activator"><span data-hover="Products">Products</span></v-text>
                <v-list>
                  <v-list-tile>
                    <v-list-tile-title class="dropdown cl-effect-5 lineheight"><nuxt-link to="/products/chargepoint"><span data-hover="ChargePoint">ChargePoint</span></nuxt-link></v-list-tile-title>
                  </v-list-tile>
                  <v-list-tile>
                    <v-list-tile-title class="dropdown cl-effect-5 lineheight"><nuxt-link to="/products/flo"><span data-hover="FLO">FLO</span></nuxt-link></v-list-tile-title>
                  </v-list-tile>
                </v-list>
        </v-menu></li>

        <li><nuxt-link to="/incentives"><span data-hover="Incentives">Incentives</span></nuxt-link></li>
        <!--<li><nuxt-link to="/partners"><span data-hover="Partners">Partners</span></nuxt-link></li>-->
            <li><v-menu open-on-hover allow-overflow auto offset-y >
              <v-text slot="activator"><span data-hover="Partners">Partners</span></v-text>
              <v-list>
                <v-list-tile>
                  <v-list-tile-title class="dropdown cl-effect-5 lineheight"><nuxt-link to="/partners#parttwo"><span data-hover="ChargePoint">ChargePoint</span></nuxt-link></v-list-tile-title>
                </v-list-tile>
                <v-list-tile>
                  <v-list-tile-title class="dropdown cl-effect-5 lineheight"><nuxt-link to="/partners#partone"><span data-hover="FLO">FLO</span></nuxt-link></v-list-tile-title>
                </v-list-tile>
              </v-list>
            </v-menu></li>
        <!--<li><nuxt-link to="/projects">Projects</nuxt-link></li>-->
        <li><nuxt-link to="/contact"><span data-hover="Contact Us">Contact Us</span></nuxt-link></li>
        <li><nuxt-link to="/general"><span data-hover="General Information">General Information</span></nuxt-link></li>
      </ul>

    </nav>
    </div>
  </header>
  <nuxt/>
  <footer>
    <div class="infobox">
      <p>20 Floral Parkway</p>
      <p>Concord, ON L4K 4R1</p>
      <br>
      <p>Tel: 905-695-1424</p>
      <p>info@ozzev.com</p>
      <br>
      <p>Follow Us:</p>
      <p>
        <!--<img src="/img/googleplus.png" alt="googleplus"/>-->
        <a href="https://www.linkedin.com/company/ozz-ev/about/" target="_blank"><img src="/img/linkedin.png" alt="linkedin"/></a></p>
      <br>
      <p>© 2019 by OZZ EV Inc. All rights reserved.</p>
    </div>
  </footer>
  </div>
  </v-app>
</template>

<style>


html {
  font-family: 'Brandon-Grotesque-light','Brandon-Grotesque-bold';
  font-size: 1rem;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;

}

.cl-effect-5 a {
  overflow: hidden;
  padding: 0 !important;
  height: 1em;
}

.cl-effect-5 a span {
  position: relative;
  display: inline-block;
  -webkit-transition: -webkit-transform 0.3s;
  -moz-transition: -moz-transform 0.3s;
  transition: transform 0.3s;
}

.cl-effect-5 a span::before {
  position: absolute;
  top: 100%;
  content: attr(data-hover);
  font-weight: 500;
  -webkit-transform: translate3d(0,0,0);
  -moz-transform: translate3d(0,0,0);
  transform: translate3d(0,0,0);
}

.cl-effect-5 a:hover span,
.cl-effect-5 a:focus span {
  -webkit-transform: translateY(-100%);
  -moz-transform: translateY(-100%);
  transform: translateY(-100%);
}

.page-enter-active, .page-leave-active {
  transition: all .6s ease-out;
}
.page-enter, .page-leave-active {
  opacity: 0;
  transform-origin: 50% 50%;
}

.v-label {
   font-size: 1rem;
    line-height: 0;
    color: black;
}

  .dropdown {
    text-align: center !important;
    /*line-height: 1rem !important;*/

  }
    .bolder {
      font-family: "Brandon-Grotesque-bold" !important;
      color: black !important;

    }

.theme__slot .v-label{
  color: black!important;
  line-height: 0 !important;
}

.v-menu {
  vertical-align: initial !important;
}

.v-card__title {
  padding: 0px !important;
}

.v-list__tile__sub-title {
  text-align: center !important;
}

.v-input__slot .v-label{
  color: black!important;
  line-height: 0 !important;
}



.content input {
  width:100%;
  /*box-sizing: border-box;*/
  font-size: 1rem;
  background-color: white;
  /*background-color: rgba(141,143,155,1);*/
  padding: 1%;
  color: rgba(141,143,155,1);
  margin: 3%;
  border: solid;
}

.content input::placeholder {
  font-size: .75rem;
  /*color: white;*/
  color: rgba(141,143,155,1);
  font-family: "Brandon-Grotesque-bold";
}

.content input[type=submit] {
  font-size: .75rem;
  color: white;
  font-family: "Brandon-Grotesque-bold";
}

.content textarea {
  width:100%;
  /*box-sizing: border-box;*/
  font-size: 1rem;
  background-color: white;
  padding: 1%;
  color: rgba(141,143,155,1);;
  margin: 3%;
  height: 6rem;
  border: solid;
}

.content textarea::placeholder {
  font-size: .75rem;
  /*color: white;*/
  color: rgba(141,143,155,1);
  font-family: "Brandon-Grotesque-bold";
}

  .requesttitle {
    font-family:"Brandon-Grotesque-bold";
    font-size: 2rem;
    color: rgba(141,143,155,1);;
  }

</style>


<script>
  import Newmenu from "~/components/Newmenu.vue";

  export default {
    components: {
      Newmenu
    },

    data () {
      return {
        dialog2: false
      }
    },

    methods: {
      bookAnInstall: function(event) {
        window.open("https://servicemaxsetrial-1634113ce9-16dcf5bfe32.force.com/lightningcust/s/", "_blank");
      }
    }

  }
</script>
