<script setup>
// Props reçues : 'tache' (objet avec id, titre, terminee)
// Événements émis : 'terminer', 'supprimer', 'modifier'
defineProps({
  tache: Object
})

const emit = defineEmits(['terminer', 'supprimer', 'modifier'])
</script>

<template>
  <div class="todo-item">
    <input type="checkbox" />
    <span>{{ tache?.titre }}</span>
    <button>Modifier</button>
    <button>Supprimer</button>
  </div>
</template>

<style scoped>
.todo-item {
  display: flex;
  align-items: center;
  gap: 10px;
  padding: 10px;
  border: 1px solid #e0e0e0;
  border-radius: 4px;
  margin-bottom: 8px;
  background-color: #fafafa;
}

span {
  flex: 1;
  font-size: 14px;
}

button {
  padding: 4px 10px;
  background-color: #f44336;
  color: white;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  font-size: 12px;
}
</style>
