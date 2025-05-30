<template>
  <div
    class="bg-stone-400 border-2 border-gray-900 rounded-xl shadow p-6 cursor-pointer hover:shadow-lg transition-shadow duration-300"
    @click="toggle">
    <h3 class="text-xl font-semibold mb-2">{{ title }}</h3>
    <p class="text-gray-700">{{ summary }}</p>

    <!-- Transição para o conteúdo expandido -->
    <transition name="fade">
      <p v-if="isOpen" class="text-gray-900 mt-4">{{ details }}</p>
    </transition>
  </div>
</template>

<script setup>
const props = defineProps({
  title: String,
  summary: String,
  details: String,
  isOpen: Boolean,
})

const emit = defineEmits(['toggle'])
function toggle() {
  emit('toggle')
}
</script>

<style scoped>
.fade-enter-active, .fade-leave-active {
  transition: all 0.3s ease;
}
.fade-enter-from, .fade-leave-to {
  opacity: 0;
  max-height: 0;
  transform: scaleY(0.95);
}
.fade-enter-to, .fade-leave-from {
  opacity: 1;
  max-height: 1000px;
  transform: scaleY(1);
}
</style>