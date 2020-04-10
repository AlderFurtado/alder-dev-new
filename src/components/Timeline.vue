<template >
  <div style="background-color: #D4E0FF" class="py-3 mt-12">
    <h1 class="display-5 font-weight-light my-6 ml-12 text-center">Historico</h1>

    <v-timeline>
      <v-timeline-item v-for="n in itens" :key="n" color="#0047FA" large class="px-md-12">
        <template v-slot:opposite>
          <span>{{ n.etapa }}</span>
        </template>
        <v-hover>
          <template v-slot="{ hover }">
            <v-card :elevation="hover ? 24 : 6">
              <v-card-title class="headline">{{ n.nome }}</v-card-title>
              <v-card-text>{{ n.descricao }}</v-card-text>
            </v-card>
          </template>
        </v-hover>
      </v-timeline-item>
    </v-timeline>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import Component from "vue-class-component";

@Component({})
export default class Timeline extends Vue {
  itens = [
    {
      nome: "CESUPA - Centro Universitario do Estado do Pará",
      descricao:
        "Instituição de ensino a qual obtive grande parte da minha formação tecnina e profissional, tal como onde eu alcancei o diploma de bacharelado em Ciência da Computação",
      etapa: "Graduação"
    },
    {
      nome: "GETA - Grupo de Estudo em Tecnologia Assistiva",
      descricao:
        "Grupo focado em tecnologia para pessoas portadoras de alguma deficiência, onde trabalhei em projetos da causa, tal como, projetos em âmbito social",
      etapa: "Grupo de estudos"
    },
    {
      nome:
        "PRODEPA - Empresa de Tecnologia da Informação e Comunicação do Estado do Pará",
      descricao:
        "Empresa de tecnologia de porte estadual, onde obtive experiência em desenvolvimento mobile, tal como, experiência em funcionamento de uma empresa de grande porte",
      etapa: "Estagio"
    },
    {
      nome: "SERPRO - Serviço Federal de Processamento de Dados",
      descricao:
        "Empresa de tecnologia de porte federal, onde obtive experiência em desenvolvimento web, tal como, experiência nas etapas de construção de software",
      etapa: "Estagio"
    }
  ];
}
</script>