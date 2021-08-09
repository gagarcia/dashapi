<template>
<div class="container full-height">
  <div class="row justify-around no-wrap q-gutter-md">
    <div>
        <q-card class="my-card q-pa-sm">
            <div class="column">
                <div>
                    <p class="text-weight-thin">Cotações Mensal</p>
                </div>
                <div>
                    <p class="text-weight-bold">R$80.000,00</p>
                </div>
                <div><PctVar variacao="2.31" /></div>
            </div>
        </q-card>
    </div>
    <div>
        <q-card class="my-card q-pa-sm">
            <div class="column">
                <div>
                    <p class="text-weight-thin">Cotações Diárias</p>
                </div>
                <div>
                    <p class="text-weight-bold">R$80.000,00</p>
                </div>
                <div><PctVar variacao="-3.12" /></div>
            </div>
        </q-card>
    </div>
    <div>
        <q-card class="my-card q-pa-sm">
            <div class="column">
                <div>
                    <p class="text-weight-thin">Cotações Hora</p>
                </div>
                <div>
                    <p class="text-weight-bold">R$80.000,00</p>
                </div>
                <div><PctVar variacao="4.16" /></div>
            </div>
        </q-card>
    </div>
  </div>
</div>
</template>

<script>
import PctVar from './PctVar.vue'

export default {
  components: {
    PctVar
  },
  data () {
    return {
    }
  }
}
</script>
