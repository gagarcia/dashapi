<template>
    <q-chip class="sinal" v-bind:color="cor">
      <div class="text-weight-bold">{{ variacao }}%</div>
    </q-chip>
</template>

<script>
export default {
  name: 'PctVar',
  props: {
    variacao: {
      type: String,
      default: 'N/A'
    }
  },
  methods: {
    isNegative (variacao) {
      const varicaoFloat = parseFloat(variacao)
      if (varicaoFloat >= 0) {
        return 'green-12'
      } else {
        return 'red-12'
      }
    }
  },
  data () {
    return {
      cor: this.isNegative(this.variacao)
    }
  }
}

</script>
