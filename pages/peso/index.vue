<template>
  <div class="text-white text-center text-2xl block bg-gradient-to-br from-black to-gray-700 h-screen block">
    Digite seu peso em Kg:
    <InputForm :placeholder="'Peso'" :value="peso" :label="'Peso'" v-model="peso"/>
    <div class="grid grid-cols-2 gap-1 h-32" style="border:1px solid red">
      <div>
        <button class=" h-full w-4/5 transition-colors duration-150 text-blue-700 border border-blue-500 rounded-lg focus:shadow-outline hover:bg-blue-600 hover:border-blue-400 hover:text-white "> 
          <span class="icon">
            <font-awesome-icon :icon="['fa', 'angles-left']" class="text-6xl"></font-awesome-icon>
          </span>
        </button>
      </div>
      <div>
        <button class=" h-full w-4/5 transition-colors duration-150 text-blue-700 border border-blue-500 rounded-lg focus:shadow-outline hover:bg-blue-600 hover:border-blue-400 hover:text-white "> 
          <span class="icon">
            <font-awesome-icon :icon="['fa', 'angles-right']" class="text-6xl"></font-awesome-icon>
          </span>
        </button>
      </div>
    </div>
  </div>
</template>

<script>
import InputForm from '../../components/Ui/InputForm.vue'

export default {
  name: 'peso',
  data() {
    return {
      peso: null,
    }
  },
  components: {
    InputForm,
  },
}
</script>

<style>

</style>