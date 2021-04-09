<template>
  <div><li>
    <span>
      <input type="checkbox">
      <strong>{{todo.id}}</strong>
      {{ todo.title }}
      </span>
    <button>&times;</button>
  </li>
  </div>
</template>

<script>
import TodoItem from '@/components/TodoItem'

export default {
  props: {
    todo: {
      type: Object,
      required: true
    }
  }

}
</script>

<style scoped>
li{
  border: 1px solid #ccc;
  display: flex;
  justify-content: space-between;
  padding: .5rem 2rem;
  margin-bottom: 1rem;
}

</style>