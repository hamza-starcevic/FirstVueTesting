<script>
export default {
  data() {
    return {
      tasks: ["Finish this"],
    };
  },
  methods: {
    addTask(task) {
      if (task !== "" && task !== " ") {
        this.tasks.push(task);
        this.task = "";
      } else return;
    },
    removeTask(task) {
      let counter = 0;
      this.tasks.map((x) => {
        console.log();
        if (x === task) this.tasks.splice(counter, 1);
        counter++;
      });
    },
  },
};
</script>

<template>
  <form id="forma" @submit.prevent="addTask(task)">
    <input type="text" v-model="task" />
    <button>Add!</button>
  </form>
  <ul>
    <li v-for="task in tasks" :key="task" :id="task">
      {{ task }} <button @click="removeTask(task)">Remove</button>
      <hr />
    </li>
  </ul>
</template>

<style>
hr {
  opacity: 0;
}

button {
  font-size: 2rem;
  color: #082336;
  width: 5em;
  height: 2em;
  border: none;
  background-color: #33ff70;
  text-decoration: none;
}

#forma {
  width: 70%;
  margin-left: 15%;
}

input {
  font-size: 2em;
  border: none;
  width: 17em;
  height: 2em;
  margin-right: 1em;
}
</style>
