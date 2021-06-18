<template>
  <nav class="container-fluid">
    <!-- SECTION Desktop -->
    <div class="row text-white p-2 mobile-gone">
      <div class="col">
        <router-link :to="{ name: 'Home' }" class="text-white">
          <span class="logo-font">Payton's Portfolio</span>
        </router-link>
      </div>

      <div class="col d-flex justify-content-end align-items-center">
        <router-link :to="{ name: 'About' }" class="text-white">
          <button type="button" class="btn btn-outline-light">
            Contact Payton
          </button>
        </router-link>
      </div>
    </div>
    <!-- SECTION Mobile -->
    <div class="row text-white p-2 desktop-gone text-center">
      <div class="col">
        <router-link :to="{ name: 'Home' }" class="text-white">
          <span class="logo-font">Payton's Portfolio</span>
        </router-link>
      </div>
    </div>
    <div class="row desktop-gone pb-3">
      <div class="col d-flex flex-column justify-content-end align-items-center">
        <router-link :to="{ name: 'About' }" class="text-white">
          <button type="button" class="btn btn-outline-light btn-lg mt-2">
            Contact Payton
          </button>
        </router-link>
      </div>
    </div>
  </nav>
</template>

<script>
import { useRoute } from 'vue-router'

export default {
  name: 'Navbar',
  setup() {
    const route = useRoute()
    return {
      route
    }
  }
}

</script>

<style scoped>
.logo-font{
  font-family: 'Montserrat', sans-serif;
  font-size: 2rem;
}

</style>
