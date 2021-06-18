<template>
  <div class="container-fluid d-flex justify-content-center m-3 m-md-5">
    <div class="row justify-content-center align-items-center">
      <!-- -->
      <router-link :to="{ name: 'Resume' }" class="text-white">
        <div class="col d-flex justify-content-center align-items-center mt-3 mt-md-0">
          <div class="card box-button box-hover no-select bg-gem-black">
            <div class="card-body d-flex justify-content-center align-items-center text-white">
              <h3 class="logo-font card-title">
                RESUME
              </h3>
            </div>
          </div>
        </div>
      </router-link>
      <!-- -->
      <router-link :to="{ name: 'Applications' }" class="text-white">
        <div class="col d-flex justify-content-center align-items-center mt-3 mt-md-0">
          <div class="card box-button box-hover no-select bg-gem-green">
            <div class="card-body d-flex justify-content-center align-items-center text-white">
              <h4 class="logo-font card-title">
                APPLICATIONS
              </h4>
            </div>
          </div>
        </div>
      </router-link>
      <!-- -->
      <router-link :to="{ name: 'About' }" class="text-white">
        <div class="col d-flex justify-content-center align-items-center mt-3 mt-md-0">
          <div class="card box-button box-hover no-select bg-gem-gray">
            <div class="card-body d-flex justify-content-center align-items-center text-white">
              <h3 class="logo-font card-title">
                CONTACT
              </h3>
            </div>
          </div>
        </div>
      </router-link>
      <!-- -->
    </div>
  </div>
</template>

<script>
export default {
  name: 'Home'
}
</script>

<style scoped lang="scss">
.box-button{
  width: 15rem;
  height: 15rem;
}
.bg-gem-green{
  background-image: url(../assets/img/gemBox1.png);
}
.bg-gem-gray{
  background-image: url(../assets/img/gemBox2.png);
}
.bg-gem-black{
  background-image: url(../assets/img/gemBox3.png);
}
.box-offline{
  width: 15rem;
  height: 15rem;
  opacity: 25%;
}
.box-hover:hover{
  cursor: pointer;
  opacity: 90%;
}
.box-hover:active{
  opacity: 80%;
}

</style>
