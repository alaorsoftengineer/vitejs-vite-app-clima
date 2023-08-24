<template>
  <Cabecalho>
    <template v-slot:Subtitulo>
      <h2>Subtitulo Aqui</h2>
    </template>

    <template v-slot:Extra>
      <h3>Texto Extra</h3>
    </template>
  </Cabecalho>

  <ListaCidades />
</template>

<script>
import './assets/estilo.css';
import Cabecalho from './components/Cabecalho.vue';
import ListaCidades from './components/ListaCidades.vue';

export default {
  components: { Cabecalho, ListaCidades },

  methods: {},
  computed: {},
};
</script>
