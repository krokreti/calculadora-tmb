<template>
    <div class="w-full sm:w-2/5 border border-gray-500 rounded-lg p-4">
        <label class="flex my-2" for="formInput">{{ label }}</label>
        <input
        :placeholder="placeholder" 
        :value="value"
        v-on="inputListeners"
        class=" 
        bg-gradient-to-br from-black to-gray-700
        w-full h-10 px-3 text-base 
        placeholder-gray-400 border 
        border-blue-500 rounded-lg 
        text-white
        focus:shadow-outline" type="text" id="formInput"/>
    </div>
</template>

<script>
export default {
    name: 'InputForm',
    props: {
        value: {
        type: [String, Number],
        default: undefined,
        },
        placeholder: {
        type: String,
        default: undefined,
        },
        label: null,
    },
    
    data() {
    return {
      localValue: this.value,
    };
  },

  watch: {
    value(value) {
      this.localValue = value;
    },
  },

  computed: {
    inputListeners() {
      const vm = this;
      return {
        ...this.$listeners,
        input(event) {
          vm.$emit('input', event.target.value);
        },
      };
    },
  },
}
</script>

<style scoped>

</style>