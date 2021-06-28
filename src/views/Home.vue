<template>
  <form>
    <input 
      type="text"
      class="form-control my-2"
      placeholder="Input name"
      v-model="task.name"
    >
    <p>{{ task }}</p>
  </form>
</template>

<script>

export default {
  name: 'Home',
  data() {
    return {
      task: {
        name: ''
      }
    }
  },
}
</script>
