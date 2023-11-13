<template>
  <input type="checkbox" :value="value" @click="toggleCheck">
</template>

<script>
export default {
  props: ['value'],

  methods: {
    toggleCheck() {
      this.$emit('input', !this.value);
    }
  }
}
</script>