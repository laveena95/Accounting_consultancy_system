<template>
  <div id="app">
      <transition appear="" name="slide-in">
        <h1>gallery</h1>
      </transition>
      <div class="grid-wrapper">
                  <v-card v-for="item in cards" :key="item.img" class="mx-auto" width="200" height="200">
                    <v-img :src="item.img" size="100">
                    </v-img>
                </v-card>
      </div>
  </div>
</template>

<script>
export default {
 data: () => {
     return{
         cards: [
                {img: require('../assets/img/1.jpg'), grid: 'card-2-1'},
                {img: require('../assets/img/2.jpg'), grid: 'card-1-1'},
                {img: require('../assets/img/3.jpg'), grid: 'card-1-1'},
                {img: require('../assets/img/4.jpg'), grid: 'card-2-1'},
                {img: require('../assets/img/5.jpg'), grid: 'card-1-1'},
                {img: require('../assets/img/1.jpg'), grid: 'card-1-1'},
         ]
     }
 }
}
</script>

<style lang="scss" scoped>
 * {
     font-size: 1rem;
     padding: 0;
     margin: 0;
     box-sizing: border-box;
}
h1 {font-size: 2rem;}

body{
    width: 100%;
    font-family: 'Segoe UI', Tahoma;
    background-color: #efefef;
    color: #333;
}
#app {
    position: relative;
    padding: 10px;
    width: 100%;
    min-height: 100vh;
}
.slide-in-enter {
    opacity: 0;
    transform: scale(0.5);
}
.slide-in-enter-active{
    transition: all .4s ease;
}
.card-1-1{
    grid-column: span 1;
}
.card-2-1{
    grid-column: span 2;
}
.grid-wrapper {
    display: grid;
    grid-template-columns: repeat(2,1fr);
    grid-gap:10px;
}
</style>