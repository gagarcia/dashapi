<template>
    <div class="container">
            <div class="column">
                <div class="text-h6">APIs</div>
                <div>
                    <div><Api titulo="Auto" subtitulo="Parceiro Multimercado" variacao="-2,12" cotacoes="80,000"/></div>
                    <div class="q-pt-sm"><Api titulo="RF" subtitulo="Seguro Incendio" variacao="2,90" cotacoes="20,000"/></div>
                    <div class="q-pt-sm"><Api titulo="Carro Fácil" subtitulo="Carro Fácil" variacao="1,22" cotacoes="20,000" /></div>
                </div>
            </div>
    </div>
</template>

<script>
import Api from './Api.vue'

export default {
  components: {
    Api
  }
}

</script>
