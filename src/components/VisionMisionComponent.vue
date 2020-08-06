<template>
   <v-layout row align-center justify-center class="mt-8">
        <v-col cols="12" md="7" v-for="item in items" :key="item.id">
            <v-card flat color="" outlined class="">
            <v-card-title primary-title class=" mt-n8 "><hr style="width:70px; height: 3px; background-color: cyan;"><h2 class="mx-2" style="">{{ item.title }}</h2></v-card-title>
            <v-crad-text> <p class="body-2 ma-5">{{ item.text }}</p> </v-crad-text>
            </v-card>
            <v-progress-linear
                buffer-value="55"
                color="cyan"
                reverse
                stream
                value="30"
                ></v-progress-linear>
        </v-col>
        <v-col cols="12" md="7" >
            <v-card flat color="" outlined class="my-5">
            <v-card-title primary-title class=" mt-n8 "><hr style="width:50px; height: 3px; background-color: cyan;"><h2 class="mx-2" style=""> OUR STRENGTHS</h2></v-card-title>
                  <v-list v-for="s in strengths" :key="s.id" dense>
                    <v-list-item>
                    <v-list-item-avatar size="10" color="cyan darken-1"></v-list-item-avatar>
                    <v-list-item-content>
                        <v-list-item-title class="nl-n2">{{ s.info }}</v-list-item-title>
                    </v-list-item-content>
                    </v-list-item>
                </v-list>
                  <v-progress-linear
                buffer-value="55"
                color="cyan"
                reverse
                stream
                value="30"
                ></v-progress-linear>
            </v-card>
          
        </v-col>
   </v-layout>
</template>

<script>
export default {
    data: () => {
        return {
            items: [
                {
                    id: '1',
                    icon: 'mdi-eye',
                    title: 'OUR VISION',
                    text: "Consectetur adipiscing elit, sued do eiusmod tempor ididunt udfgt labore et dolore magna aliqua. Quis ipsum suspendisces gravida. Risus commodo viverra sebfd dho eiusmod tempor maecenas accumsan lacus. Risus commodo viverra sebfd dho eiusmod tempor maecenas accumsan lacus.",
                    text2: "Risus commodo viverra sebfd dho eiusmod tempor maecenas accumsan lacus. Risus commodo viverra sebfd dho eiusmod tempor maecenas accumsan.", 
                    },
                {
                    id: '2',
                    icon: 'mdi-magnify',
                    title: 'OUR MISSION',
                    text: "Consectetur adipiscing elit, sued do eiusmod tempor ididunt udfgt labore et dolore magna aliqua. Quis ipsum suspendisces gravida. Risus commodo viverra sebfd dho eiusmod tempor maecenas accumsan lacus. Risus commodo viverra sebfd dho eiusmod tempor maecenas accumsan lacus.",
                    text2: "Risus commodo viverra sebfd dho eiusmod tempor maecenas accumsan lacus. Risus commodo viverra sebfd dho eiusmod tempor maecenas accumsan.", 
                    },
            ],
            strengths: [
                {
                    id : '1',
                    info : "Professional and competent staff",
                },
                {
                    id : '2',
                    info : "Direct and simple processes for communicating with our customers",
                },
                {
                    id : '3',
                    info : "The ability to work flexibly in cooperation with companies and organizations of all sizes, regardless of their field",
                },
                {
                    id : '4',
                    info : "Modern electronic systems",
                },
            ]
        }
    }
}
</script>

<style>

</style>