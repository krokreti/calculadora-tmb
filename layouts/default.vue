<template>
  <div class="principal h-screen w-full bg-fixed bg-no-repeat ">
    <div class="container mx-auto w-full h-screen sm:h-4/5 sm:w-4/5">
      <Nuxt />
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
.principal {
  background-image: url('../static/gymwp.jpg');
  background-size: 100%;
  
  
}

@media (max-width: 600px) {
      .principal {
        background-position: -630px -0px;
        background-size: cover;
      }
}


</style>