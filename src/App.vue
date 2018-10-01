<template>
  <div>
    <label id="fruitLabel">Choose a fruit: </label>
    <Autocomplete :items="[ 'Apple', 'Banana', 'Orange', 'Mango', 'Pear', 'Peach', 'Grape', 'Tangerine', 'Pineapple']" aria-labelled-by="fruitLabel" />

    <br>
    <hr>
    <br>

    <label id="cityLabel">עיר:</label>
    <Autocomplete :items="['חיפה','יקנעם-עילית','תל-אביב','רמת-גן','נשר','נתניה']" aria-labelled-by="cityLabel" :placeholder="`בחר עיר`"/>
  </div>
</template>

<script>
import Autocomplete from './components/autocomplete'

export default {
  name: 'App',
  components: {
    Autocomplete
  }
}
</script>

<style>
@import "./scss/font-open-sans-hebrew.css";
#app {
  font-family: 'Open Sans Hebrew', Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
#fruitLabel, #cityLabel {
  box-sizing: border-box;
  color: rgb(91, 98, 101);
  cursor: default;
  direction: rtl;
  display: block;
  font-family: 'Open Sans Hebrew';
  font-size: 16px;
  height: 18px;
  line-height: 18.4px;
  user-select: none;
  width: 258px;
}
</style>
