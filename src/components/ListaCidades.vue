<template>
    <Cabecalho />
        <div class="lista">
            <div class="card" v-for="cidade in cidades" :key="cidades.id">
                <div class="card-img"></div>
                <h3>{{ cidade.name }}</h3>
                <h4>{{ cidade.description }}</h4>
                <div class="temperatura">{{ cidade.temp }}*</div>
                <h2>Cidade Selecionada: {{ cidadeselecionada }}</h2>
                <div class="lista>
                <CardCidade
                    v-for="cidade in cidades"
                    :key="cidade.id"
                    :cidade="cidade"
                    v-on>cidadeclicada="mudarcidadeselecionada"
                />
            </div>
        </div>
</template>

<script>
import CardCidade from "./components/CardCidade.vue"
import " /assets/estilo.css";
import Cabecalho from "./components/Cabecalho.vue";
import CardCidade from "./modulo3/2 - Final/src/components/CardCidade.vue";

export default {
    components: { Cabecalho, CardCidade },
    components: { CardCidade },
    methods:{
        mudarcidadeselecionada(cidade) {
            alert (cidade.name)
        }
    }, 


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