<template>
  <div>
    <app-header></app-header>
    <app-programmer></app-programmer>
    <app-footer></app-footer>
  </div>
</template>

<script>

import Header from './components/Header'
import Footer from './components/Footer'
import Programmer from "./components/Programmers";

export default {
  components: {
    'app-header': Header,
    'app-footer': Footer,
    'app-programmer': Programmer
  },
  data() {

  }
}
</script>

<style>

body {
  margin: 0;
}

</style>
