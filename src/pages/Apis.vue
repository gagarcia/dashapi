<template>
  <q-page>
      <div class="container q-pa-sm"><ListaApis /></div>
  </q-page>
</template>

<script>
import { defineComponent } from 'vue'
import ListaApis from '../components/ListaApis.vue'

export default defineComponent({
  name: 'PageIndex',
  components: {
    ListaApis
  }
})
</script>

<style scoped>
  .text-brand {
    color: #30c5ff;
  }
</style>
