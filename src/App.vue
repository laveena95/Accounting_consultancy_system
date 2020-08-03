<template>
  <v-app>
   <ReasonComponent/>
   <ReferenceComponent/>
   <CalComponent/>
   <test/>
  </v-app>
</template>

<script>
import ReasonComponent from './components/ReasonComponent';
import ReferenceComponent from './components/ReferenceComponent';
import CalComponent from './components/CalComponent';
import test from './components/test';

export default {
  name: 'App',

  components: {
    ReasonComponent,
    ReferenceComponent,
    CalComponent,
    test,
  },

  data: () => {
      return {
         
      }
      }
};
</script>
