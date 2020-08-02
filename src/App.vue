<template>
  <v-app>
   <ReasonComponent/>
   <ReferenceComponent/>
   <CalComponent/>
  </v-app>
</template>

<script>
import ReasonComponent from './components/ReasonComponent';
import ReferenceComponent from './components/ReferenceComponent';
import CalComponent from './components/CalComponent';

export default {
  name: 'App',

  components: {
    ReasonComponent,
    ReferenceComponent,
    CalComponent,
  },

  data: () => ({
    //
  }),
};
</script>
