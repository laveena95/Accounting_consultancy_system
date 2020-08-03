<template>
<v-container fluid>
    <div>
        <h1 class="text-center font-weight-regular;">CHECK OUR REFERENCES</h1>
    </div>
        <h2 class="body-1 text-center">
            Our clientele includes a diverse group of partnerships, limited liability companies, associations and foundations, and our customer turnover is limited.
        </h2>
    <v-row class="ma-3 ">
        <v-col cols="12" md="4" sm="4" v-for="item in items" :key="item.id">
                <v-hover v-slot:default="{ hover }">
                    <v-card
                    class="mx-auto"
                    color="grey lighten-4"
                    >
                    <v-img
                        :aspect-ratio="16/9"
                        :src="item.img"
                    >
                        <v-expand-transition>
                            
                        <div
                            v-if="hover"
                            class="d-flex transition-fast-in-fast-out white darken-2 v-card--reveal display-3 black--text ma-2"
                            style="height: 94%;"
                        >
                            <p class="body-1 text-center" absolute> {{ item.text}} </p>
                        </div>
                        </v-expand-transition>
                    </v-img>
                    </v-card>
                </v-hover>
        </v-col>
    </v-row>
</v-container>
</template>

<script>
    export default {
        data () {
            return {
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
            }
        }
    }
</script>


<style>
.v-card--reveal {
  align-items: center;
  bottom: 0;
  justify-content: center;
  opacity: .7;
  position: absolute;
  width: 100%;
}
</style>