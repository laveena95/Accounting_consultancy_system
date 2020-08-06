<template>
  <v-app>
   <ReasonComponent/>
   <ReferenceComponent/>
   <CalComponent/>
   <VisionMissionComponent/>
   <CareerBanner/>
   <welcome/>
   <story/>
    <test/>
   
  </v-app>
</template>

<script>
import ReasonComponent from './components/ReasonComponent';
import ReferenceComponent from './components/ReferenceComponent';
import test from './components/test';
import CalComponent from './components/CalComponent';
import VisionMissionComponent from './components/VisionMisionComponent';
import CareerBanner from './components/CareerBanner'
import welcome from './components/welcome';
import story from './components/story';

export default {
  name: 'App',

  components: {
    ReasonComponent,
    ReferenceComponent,
    test,
    CalComponent,
    VisionMissionComponent,
    CareerBanner,
    welcome,
    story,
  },

  data: () => {
      return {
         
      }
      }
};
</script>
