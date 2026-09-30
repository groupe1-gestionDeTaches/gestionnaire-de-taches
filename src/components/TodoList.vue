<script setup>
import TodoItem from './TodoItem.vue'

// Props reçues : 'tâches' (tableau d'objets)
// Événements émis : 'terminer', 'supprimer', 'modifier'
defineProps({
  tâches: Array
})

const emit = defineEmits(['terminer', 'supprimer', 'modifier'])
</script>

<template>
  <div class="todo-list">
    <slot>
      <!-- Par défaut, affiche les tâches avec TodoItem -->
    </slot>
  </div>
</template>

<style scoped>
.todo-list {
  min-height: 100px;
}
</style>
