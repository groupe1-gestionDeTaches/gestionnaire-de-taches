<script setup>
// Événements émis : 'filtrer' (avec le statut choisi)
const emit = defineEmits(['filtrer'])
</script>

<template>
  <div class="todo-filter">
    <button>Toutes</button>
    <button>À faire</button>
    <button>Terminées</button>
  </div>
</template>

<style scoped>
.todo-filter {
  display: flex;
  gap: 5px;
  margin-bottom: 15px;
  border-bottom: 1px solid #e0e0e0;
  padding-bottom: 10px;
}

.todo-filter button {
  padding: 6px 12px;
  background-color: transparent;
  color: #666;
  border: 1px solid #ddd;
  border-radius: 4px;
  cursor: pointer;
  font-size: 13px;
}
</style>
