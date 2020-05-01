<template>
  <div id="app">
    <v-header></v-header>
    <v-button>Contact</v-button>
    <v-button>Hire Me</v-button>
    <v-text></v-text>
    <div class="img-grid">
      <v-img></v-img>
      <v-img></v-img>
      <v-img></v-img>
      <v-img></v-img>
      <v-img></v-img>
      <v-img></v-img>
    </div>
    
  </div>
</template>

<script>
import Header from 'Components/Header'
import Button from 'Components/Button'
import Img from 'Components/Img'
import textBlock from 'Components/textBlock'

export default {
  name: 'app',
  components: {
    'v-header': Header,
    'v-button': Button,
    'v-img': Img,
    'v-text': textBlock
  },
  methods: {
     consoleClick() {
      console.log('Button clicked')
    }
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css?family=Roboto+Slab');
@import url('https://fonts.googleapis.com/css?family=Questrial');


html, body, div, span, applet, 
h1, h2, h3, h4, h5, h6, p, blockquote, pre, a 
{
  margin: 0;
  padding: 0;
  border: 0;
  font-size: 100%;
  font: inherit;
  vertical-align: baseline;
  font-family:'Courier New', Courier, monospace;
  margin-top: 2em;
}

.img-grid {

  display: flex;
  flex-wrap: wrap;
  margin: 0 auto;
  width: 100%;
  justify-content:center;
  margin-top: 3em;
}

html {
  box-sizing: border-box;
}

*, *:before, *:after {
  box-sizing: inherit;
  outline: none;
}

#app {

  text-align: center;
  color: #fff;
  margin-top: 60px;
}

body {
  background: #22264b;
  font-family: 'Roboto Slab', serif;
}

h1, h2, h3, h4, h5, h6 {
  color: #e6cf8b;
  font-weight: bold;
  font-family: 'Questrial', sans-serif;
}

h1 {
  font-size: 3em;
}

h2 {
  font-size: 2.25em;
}

h3 {
  font-size: 1.75em;
}

button, input, textarea {
  font-family: 'Roboto Slab', serif;
}
</style>
