<template>
  <div>
      <v-row>
          <v-col cols="12" md="6">
               <NumberInputSpinner
                :min="0"
                :max="10"
                :step="10"
                :integerOnly="true"
                v-model="yourVModel"
                size="small"
                />
          </v-col>
      </v-row>
  
  </div>
</template>

<script>
  import NumberInputSpinner from 'vue-number-input-spinner'

export default {
  components: {
    NumberInputSpinner,
  },
}
</script>