<template>
  <div class=" w-full h-full flex align-between justify-center">
    <div class="grid grid-cols-1 gap-1">
      <div class="grid grid-rows-1 ">
        <div class="font-sans text-white p-4 text-3xl sm:text-5xl text-center" >Descubra sua taxa metabólica basal!</div>
      </div>
      <div class="grid grid-rows-1 text-white h-11 px-4 sm:flex sm:justify-center" >
        <nuxt-link to="/sexo">
          <button class="w-full sm:w-min text-white transition-colors duration-150 bg-green-500 sm:rounded-lg focus:shadow-outline hover:bg-gray-800 px-4 py-2 shadow  " >Começar</button>
        </nuxt-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Index',
  layout: 'default',
}
</script>

<style>

</style>