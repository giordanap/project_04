<template>
  <form>
    
    <input 
      type="text"
      class="form-control my-2"
      placeholder="Input name"
      v-model="task.name"
    >
    <div class="form-check form-check-inline">
      <input 
        type="checkbox" 
        id="check-1 "
        class="form-check-input"
        v-model="task.categories"
        value="javascript"
      >
      <label for="check-1" class="form-check-label"> Javascript </label>
    </div>
    <div class="form-check form-check-inline">
      <input 
        type="checkbox" 
        id="check-1 "
        class="form-check-input"
        v-model="task.categories"
        value="node js"
      >
      <label for="check-1" class="form-check-label"> Node.js </label>
    </div>
    <div class="form-check form-check-inline">
      <input 
        type="checkbox" 
        id="check-1 "
        class="form-check-input"
        v-model="task.categories"
        value="python"
      >
      <label for="check-1" class="form-check-label"> Python </label>
    </div>
    <div class="form-check form-check-inline">
      <input 
        type="checkbox" 
        id="check-1 "
        class="form-check-input"
        v-model="task.categories"
        value="c#"
      >
      <label for="check-1" class="form-check-label"> C# </label>
    </div>

    <div class="mt-2">

      <div class="form-check form-check-inline">
        <input 
          type="radio"
          id="radio-1"
          class="form-check-input"
          v-model="task.state"
          value="urgent"
        >
        <label for="radio-1" class="form-check-label"> Urgent </label>
      </div>
      <div class="form-check form-check-inline">
        <input 
          type="radio"
          id="radio-2"
          class="form-check-input"
          v-model="task.state"
          value="relax"
        >
        <label for="radio-2" class="form-check-label"> Relax </label>
      </div>

    </div>


  </form>
  <hr>
  <p>
    {{ task }}
  </p>
</template>

<script>

export default {
  name: 'Home',
  data() {
    return {
      task: {
        name: '',
        categories: [],
        state: ''
      }
    }
  },
}
</script>
