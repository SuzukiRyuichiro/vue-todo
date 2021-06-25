<template>
  <div id="tasks">
    <TaskCard
      :title="tasks[0].title"
      :description="tasks[0].description"
      :done="tasks[0].done"
    ></TaskCard>
    <TaskCard
      :title="tasks[1].title"
      :description="tasks[1].description"
      :done="tasks[1].done"
    ></TaskCard>
    <TaskCard
      :title="tasks[2].title"
      :description="tasks[2].description"
      :done="tasks[2].done"
    ></TaskCard>
  </div>
</template>

<script>
  import TaskCard from './TaskCard';

  export default {
    components: { TaskCard },

    data() {
      return {
        tasks: [
          {
            title: "Create a card component",
            description:
              "Create a new TaskCard.vue file in the components folder, then import it in TasksList",
            done: true,
          },
          {
            title: "Make the card component dynamic",
            description:
              "Learn about using the data option and passing data to child components using props",
            done: true,
          },
          {
            title: "Bind the attributes to the data",
            description:
              "Use the v-bind directive to bind the title and description to our data",
            done: false,
          },
        ],
      };
    },
  }

</script>
