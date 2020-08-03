<template>
    <v-layout row align-center justify-center class="ma-1" >
            <v-card class="mt-6" width="600" height="" flat align="center" justify="center">
                <v-card-title primary-title class="layout justify-center"><h2>Laske hinta-arvio 2 minuutissa!</h2></v-card-title>
                <v-card-text class="body-2">
                    Hae yrityksesi tilanteeseen parhaiten sopiva taloushallinnon palvelu.Et sitoudu mihinkään!
                </v-card-text>
                    <v-card-content>
                        <v-form>
                            <v-container>
                                <v-row >
                                    <v-col cols="12" sm="6" >
                                          <v-input>
                                               MYYNTI EUROINA / VUOSI
                                               <v-tooltip right>
                                            <template v-slot:activator="{ on, attrs }">
                                                <v-btn
                                                color="primary"
                                                class="mt-n8" fab dark x-small
                                                v-bind="attrs"
                                                v-on="on"
                                                > <v-icon v-on="on">mdi-help-circle-outline</v-icon></v-btn>
                                            </template>
                                            <span >
                                                <p class="caption" style="width:100px;">
                                                    Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s.
                                                </p>
                                            </span>
                                            </v-tooltip>
                                            </v-input>
                                    </v-col>
                                      <v-col  cols="12" sm="6">
                                        <v-select
                                        :items="items"
                                         label="select your range"
                                        placeholder="Ex: 75,000 - 100,000"
                                        rounded
                                        outlined
                                        ></v-select>
                                    </v-col>
                                </v-row>
                                <v-row>
                                    <v-col cols="12" md="4">
                                        <v-input class="caption">
                                            PALKKALASKELMAT/KK
                                            <v-tooltip right>
                                                <template v-slot:activator="{ on, attrs }">
                                                    <v-btn
                                                    color="primary"
                                                    class="mt-n8" fab dark x-small
                                                    v-bind="attrs"
                                                    v-on="on"
                                                    > <v-icon v-on="on">mdi-help</v-icon></v-btn>
                                                </template>
                                                <span >
                                                    <p class="caption" style="width:100px;">
                                                        Lorem Ipsum is simply dummy text of the printing and typesetting industry.
                                                    </p>
                                                </span>
                                            </v-tooltip>
                                        </v-input>
                                        <NumberInputSpinner
                                            :min="0"
                                            :max="10"
                                            :step="1"
                                            :integerOnly="true"
                                            v-model="yourVModel"
                                            size="small"
                                            />
                                    </v-col>
                                    <v-col cols="12" md="4">
                                        <v-input class="caption">
                                            MYYNTILASKUT/KK
                                               <v-tooltip right>
                                                    <template v-slot:activator="{ on, attrs }">
                                                        <v-btn
                                                        color="primary"
                                                        class="mt-n8" fab dark x-small
                                                        v-bind="attrs"
                                                        v-on="on"
                                                        > <v-icon v-on="on">mdi-help</v-icon></v-btn>
                                                    </template>
                                            <span >
                                                <p class="caption" style="width:100px;">
                                                    Lorem Ipsum is simply dummy text of the printing and typesetting industry.
                                                </p>
                                            </span>
                                            </v-tooltip>
                                        </v-input>
                                        <NumberInputSpinner
                                            :min="0"
                                            :max="10"
                                            :step="10"
                                            :integerOnly="true"
                                            v-model="yourVModel"
                                            size="small"
                                            />
                                    </v-col>
                                    <v-col cols="12" md="4">
                                        <v-input class="caption">
                                            OSTOLASKUT/KK
                                               <v-tooltip right>
                                            <template v-slot:activator="{ on, attrs }">
                                                <v-btn
                                                color="primary"
                                                class="mt-n8" fab dark x-small
                                                v-bind="attrs"
                                                v-on="on"
                                                > <v-icon v-on="on">mdi-help</v-icon></v-btn>
                                            </template>
                                            <span >
                                                <p class="caption" style="width:100px;">
                                                    Lorem Ipsum is simply dummy text of the printing and typesetting industry.
                                                </p>
                                            </span>
                                            </v-tooltip>
                                            </v-input>
                                        <NumberInputSpinner
                                            :min="0"
                                            :max="10"
                                            :step="1"
                                            :inputClass="alert"
                                            :buttonClass="success"
                                            :integerOnly="true"
                                            v-model="number"
                                            size="small"
                                        >
                                        </NumberInputSpinner>
                                        
                                    </v-col>
                                </v-row>
                            </v-container>
                        </v-form>
                    </v-card-content>
            </v-card>
    </v-layout>
</template>

<script>
import NumberInputSpinner from 'vue-number-input-spinner'
  export default {
       components: {
    NumberInputSpinner,
  },
    data: () => ({
     
      select: null,
      items: [
        '-',
        '0 - 75,000',
        '75,000 - 100,000',
        '100,000 - 125,000',
        '125,000 - 150,000',
        '150,000 - 200,000'
      ],
    }),
  }
</script>
<style scoped>

</style>