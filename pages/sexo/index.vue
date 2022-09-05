<template>

  <div class="text-white text-center text-2xl p-4 block bg-gradient-to-br from-black to-gray-700 h-screen">
    Escolha seu sexo:
    <div class="grid grid-cols-2 gap-1 h-3/5 flex content-center" >
      <div >
        <div class="grid-rows-1 mb-3">Masculino
        </div>
        <nuxt-link to="/peso">
        <button class=" transition-colors duration-150 text-blue-700 border border-blue-500 rounded-lg focus:shadow-outline hover:bg-blue-600 hover:border-blue-400 hover:text-white w-4/5 "> 
          <span class="icon">
            <font-awesome-icon :icon="['fas', 'mars']" class="m-4 text-9xl"></font-awesome-icon>
          </span>
        </button>
        </nuxt-link>
      </div>
      <div>
      <div class="mb-3">Feminino
      </div>
      <nuxt-link to="/peso">
        <button class="transition-colors duration-150 text-pink-700 border border-pink-500 rounded-lg focus:shadow-outline hover:bg-pink-600 hover:border-pink-400 hover:text-white w-4/5">
          <span class="icon">
            <font-awesome-icon :icon="['fas', 'venus']"  class="m-4 text-9xl"></font-awesome-icon>
        </span>
        </button>
      </nuxt-link>
      </div>
      </div>
  </div>
  
</template>

<script>
export default {
    name: 'sexo'
}
</script>

<style>

</style>