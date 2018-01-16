<template>
  <div id="app">

    <v-layout row wrap>
        <v-flex xs12 text-xs-center dark indigo>
           <v-footer  height="auto" class="d-block" >
              <v-card flat tile >
                <v-card-text class="white--text" >
                  <v-spacer></v-spacer>
                    <v-btn
                     v-for="icon in icons"
                     :key="icon"
                     icon
                     class="mx-3"

                    >
                      <v-icon size="24px">{{ icon }}</v-icon>
                    </v-btn>
                </v-card-text>

              </v-card>
              <v-card flat tile>
               <v-card-text class="white--text">
               Phasellus feugiat arcu sapien, et iaculis ipsum elementum sit amet. Mauris cursus commodo interdum. Praesent ut risus eget metus luctus accumsan id ultrices nunc. Sed at orci sed massa consectetur dignissim a sit amet dui. Duis commodo vitae velit et faucibus. Morbi vehicula lacinia malesuada. Nulla placerat augue vel ipsum ultrices, cursus iaculis dui sollicitudin. Vestibulum eu ipsum vel diam elementum tempor vel ut orci. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.
               </v-card-text>
              </v-card>
              <v-card flat tile >
                 <v-card-text class="white--text">
                    &copy; 2017 Copyright:
                    <strong>MDBootstrap.com</strong>
                    <v-spacer></v-spacer>
                </v-card-text>
              </v-card>

      </v-footer>
    </v-flex>
  </v-layout>

</div>
 </template>



<script>
  export default {
    data () {
      return {
        icons: ['fa-facebook', 'fa-twitter', 'fa-google-plus', 'fa-linkedin', 'fa-instagram'],
        clipped: false,
        drawer: true,
        fixed: false,
        items: [
          { icon: 'bubble_chart', title: 'Inspire' }
        ],
        miniVariant: false,
        right: true,
        rightDrawer: false,
        title: 'Vuetify.js'
      }
    }
  }
</script>
