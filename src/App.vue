<script setup>
import TodoForm from './components/TodoForm.vue'
import TodoFilter from './components/TodoFilter.vue'
import TodoList from './components/TodoList.vue'
</script>

<template>
  <div class="app">
    <h1>Ma Liste de Tâches</h1>

    <!-- reçoit l'événement 'ajouter' -->
    <TodoForm />

    <!-- reçoit l'événement 'filtrer' -->
    <TodoFilter />

    <!-- reçoit les tâches en props et émet 'terminer', 'supprimer', 'modifier' -->
    <TodoList />
  </div>
</template>

<style scoped>
.app {
  background: white;
  border: 2px solid #c5cae9;
  border-radius: 8px;
  padding: 20px;
}

h1 {
  color: #3f51b5;
  text-align: center;
  margin-bottom: 20px;
  font-size: 1.5rem;
}
</style>
