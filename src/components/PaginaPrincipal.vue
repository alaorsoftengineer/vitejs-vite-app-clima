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
data() {
        return {
            cidades: {
                {
                    id: 8429,
                    name: "Rio de Janeiro",
                    description: "Ensolarado",
                    icon: "01d",
                    temp: "25",
                }

                {
                    id: 8412,
                    name: "Manaus",
                    description: "Chuvas Fortes",
                    icon: "09d",
                    temp: "25",
                }

                {
                    id: 8454,
                    name: "Brasilia",
                    description: "Ensolarado",
                    icon: "10d",
                    temp: "27.4",
                }



            }
        }
}
</script>
