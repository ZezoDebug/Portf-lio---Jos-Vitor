<template>
  <section class="max-w-5xl mx-auto p-6">
    <h2 class="text-3xl font-bold text-sky-700 mb-8 text-center">Minha Trajetória</h2>

    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">

      <!-- Card 1 -->
      <ExpandableCard
        title="Ensino Médio"
        summary="Completei o ensino médio na Escola José Gonçalves de Mendonça..."
        details="Durante o ensino médio, comecei a me interessar por informática, explorando o uso dos computadores e descobrindo o quanto a tecnologia pode ser fascinante."
        :isOpen="openCard === 1"
        @mouseenter="setCard(1)"
        @mouseleave="clearCard"/>

      <!-- Card 2 -->
      <ExpandableCard
        title="Experiência Profissional"
        summary="Trabalhei como Auxiliar Administrativo na industria Raízen, adquirindo experiência..."
        details="Trabalhei como auxiliar administrativo na Raízen, onde desenvolvi habilidades organizacionais, atenção aos detalhes e aprendi mais sobre o funcionamento do ambiente corporativo."
        :isOpen="openCard === 2"
        @mouseenter="setCard(2)"
        @mouseleave="clearCard"/>

      <!-- Card 3 -->
      <ExpandableCard
        title="Cursos Extra Curriculares"
        summary="Fiz cursos de Informatica e Mecânica Industrial..."
        details="Durante minha formação, cursei informática e mecânica industrial, o que ampliou meus conhecimentos técnicos e reforçou meu interesse por tecnologia e processos industriais."
        :isOpen="openCard === 3"
        @mouseenter="setCard(3)"
        @mouseleave="clearCard"/>

      <!-- Card 4 -->
      <ExpandableCard
        title="Faculdade de ADS"
        summary="Atualmente cursando Análise e Desenvolvimento de Sistemas..."
        details="Na faculdade, estou focado em desenvolvimento web, com preferência por front-end. Tenho interesse em back-end, embora ainda encontre algumas dificuldades nessa área."
        :isOpen="openCard === 4"
        @mouseenter="setCard(4)"
        @mouseleave="clearCard"/>
    </div>
  </section>
</template>

<script setup>
import { ref } from 'vue'
import ExpandableCard from '../components/ExpandableCard.vue'

// Controla qual card está aberto (apenas um por vez)
const openCard = ref(null)

function setCard(id) {
  openCard.value = id
}

function clearCard() {
  openCard.value = null
}
</script>