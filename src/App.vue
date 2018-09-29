<template>
  <!-- <div id="app">
    <img src="./assets/logo.png">
    <HelloWorld/>
  </div> -->
  <div>
    <label id="fruitLabel">Choose a fruit: </label>
    <Autocomplete :items="[ 'Apple', 'Banana', 'Orange', 'Mango', 'Pear', 'Peach', 'Grape', 'Tangerine', 'Pineapple']" aria-labelled-by="fruitLabel" />

    <br>
    <hr>
    <br>

    <label id="cityLabel">עיר:</label>
    <Autocomplete :items="['חיפה','יקנעם-עילית','תל-אביב','רמת-גן','נשר','נתניה']" aria-labelled-by="cityLabel" />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import Autocomplete from './components/autocomplete'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Autocomplete
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
