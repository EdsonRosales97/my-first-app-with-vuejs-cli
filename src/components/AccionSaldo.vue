<template>

  <button class="btn btn-outline-dark" @click="accion" :disabled="desactivar">
      {{ texto }}
  </button>

</template>

<script>
export default {
    props: {
        texto: String,
        desactivar: {
            type: Boolean,
            default: false,
        }
    },
    methods: {
        accion() {
            this.$emit('accion');
        },
    }
}
</script>

<style>

</style>