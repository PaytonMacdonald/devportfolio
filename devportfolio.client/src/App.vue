<template>
  <header class="shadow">
    <Navbar />
  </header>
  <main class="shadow">
    <router-view />
  </main>
  <footer class="container-fluid shadow">
    <div class="row justify-content-center text-light pb-4 pt-2 pb-md-t text-center">
      208.800.9821 (call or text) <span class="mobile-gone">|</span> paytonmac49@gmail.com
    </div>
  </footer>
</template>

<script>
import { computed } from 'vue'
import { AppState } from './AppState'
export default {
  name: 'App',
  setup() {
    return {
      appState: computed(() => AppState)
    }
  }
}
</script>
<style lang="scss">
@import "./assets/scss/main.scss";
.logo-font{
  font-family: 'Montserrat', sans-serif;
}
@media only screen and (max-width:800px){
.mobile-gone{
  display: none;
}
}
@media only screen and (min-width:800px){
.desktop-gone{
  display: none;
}
}
.no-select {
  -webkit-touch-callout: none; /* iOS Safari */
    -webkit-user-select: none; /* Safari */
     -khtml-user-select: none; /* Konqueror HTML */
       -moz-user-select: none; /* Old versions of Firefox */
        -ms-user-select: none; /* Internet Explorer/Edge */
            user-select: none; /* Non-prefixed version, currently
                                  supported by Chrome, Edge, Opera and Firefox */
}
</style>
