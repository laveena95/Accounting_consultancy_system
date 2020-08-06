<template>
    <v-layout row align-center justify-center class="ma-8">
       <v-card flat="">
           <v-card-title>
               <hr style="width:40px; height: 3px; background-color: cyan;"><h1 class="text-center font-weight-regular;">CHECK OUR REFERENCES</h1>
           </v-card-title>
       </v-card>
        <h2 class="body-1 text-center ma-5">
            Our clientele includes a diverse group of partnerships, limited liability companies, associations and foundations, and our customer turnover is limited.
        </h2>
      <v-col cols="12" md="4" v-for="item in items" :key="item.id" >
        <v-hover>
            <template v-slot:default="{ hover }">
            <v-card
                class="mx-auto"
                elevation="10"
            >
                <v-img :aspect-ratio="16/9" :src="item.img"></v-img>
                <v-fade-transition>
                <v-overlay
                    v-if="hover"
                    absolute
                    color="#036358"
                >
                    <v-btn rounded="">See more info</v-btn>
                    <v-btn class="mx-2" fab dark small color="">
                        <v-icon dark>mdi-eye</v-icon>
                    </v-btn>
                </v-overlay>
                </v-fade-transition>
            </v-card>
            </template>
        </v-hover>
      </v-col>
    </v-layout>
</template>

<script>
  export default {
    data: () => ({
      overlay: false,
      items: [
                    {
                        id: '1',
                        img: require('../assets/img/1.jpg'),
                        text: 'Loreum ipsum',
                    },
                    {
                        id: '2',
                        img: require('../assets/img/2.jpg'),
                        text: 'Loreum ipsum',
                    },
                    {
                        id: '3',
                        img: require('../assets/img/3.jpg'),
                        text: 'Loreum ipsum',
                    },
                    {
                        id: '4',
                        img: require('../assets/img/4.jpg'),
                        text: 'Loreum ipsum',
                    },
                    {
                        id: '5',
                        img: require('../assets/img/5.jpg'),
                        text: 'Loreum ipsum',
                    },
                    {
                        id: '6',
                        img: require('../assets/img/6.jpg'),
                        text: 'Loreum ipsum',
                    }
                ]
    }),
  }
</script>