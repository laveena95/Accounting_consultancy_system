<template>
  <v-container >
      <v-row class="" align-content="center">
        <v-col cols="12" md="9">
          <v-card width="" flat align-center>
          <v-container >
            <div class="d-flex flex-no-wrap justify-space-between text--justify">
              <div>
                <v-card-title
                  class="headline"
                ><hr style="width:40px; height: 3px; background-color: cyan;"><h1 class="ma-3">Our Career</h1></v-card-title>
                <v-card-text>
                    <p class="body-1">
                       <b> Surfers, cheerleaders, players, chefs, daughters, boys, fathers and mothers - 2,350 accountants in 7 countries, all different and unique but all part of the a + team!</b>
                    </p>
                </v-card-text>
                <v-card-text class="body-1"><p>We at Accountor are pioneers: Curiosity, growth and development strain us because we want to be one step ahead . Accountor's open and flexible work environment is a place where there is always room for new ideas to develop . We keep our promises, set our goals high and work hard to make our customers successful. For us, Accountor is an a + job !.</p>
              </v-card-text>
              </div> 
            </div>
            <v-card-actions>
              <v-row>
                <v-col cols="12" md="3">
                  <v-btn color="black" dark class="">
                  <v-icon small color="white mx-auto ml-2">mdi-magnify</v-icon><v-sapcer> </v-sapcer>
                  Vacancies in finland</v-btn>
                </v-col>
                <v-col cols="12" md="1"></v-col>
                <v-col cols="12" md="4">
                  <v-btn color="black" dark class="">
                  <v-icon small color="white">mdi-users</v-icon><v-spacer> </v-spacer>
                 recent graduates</v-btn>
                </v-col>
              </v-row>
              </v-card-actions>
          </v-container>
          </v-card>
        </v-col>
        <v-col cols="12" md="3" class="mt-12 hidden-sm">
          <v-card flat elevation="10" shaped="">
             <v-avatar
                class=""
                size="300"
              >
                <img src="../assets/img/c1.jpg" alt="" class="">
              </v-avatar>
          </v-card>
        </v-col>
        
      </v-row>
  </v-container>
</template>

<script>
export default {
    name: 'Info'
}
</script>

 <style scoped>
 a{
   text-decoration: none;
   color:turquoise;
   font-weight: 500;
 }
 </style>