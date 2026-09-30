<script setup>
// Événements émis : 'ajouter' (avec le texte de la tâche)
const emit = defineEmits(['ajouter'])
</script>

<template>
  <div class="todo-form">
    <input type="text" placeholder="Nouvelle tâche..." />
    <button>Ajouter</button>
  </div>
</template>

<style scoped>
.todo-form {
  display: flex;
  gap: 10px;
  margin-bottom: 15px;
}

input {
  flex: 1;
  padding: 10px;
  border: 1px solid #c5cae9;
  border-radius: 4px;
  font-size: 14px;
}

button {
  padding: 10px 20px;
  background-color: #3f51b5;
  color: white;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}
</style>
