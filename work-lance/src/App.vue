<script>
export default {
  data() {
    return {
      name: "Elise Lee",
      status: "active",
      tasks: ["Task One", "Task Two", "Task Three"],
      link: "https://google.com",
    };
  },
};
</script>

<template>
  <h1>{{ name }}</h1>
  <p v-if="status === 'active'">User is active</p>
  <p v-else-if="status === 'pending'">User is pending</p>
  <p v-else>User is inactive</p>

  <h3>Tasks:</h3>
  <ul>
    <li v-for="task in tasks" :key="task">{{ task }}</li>
  </ul>
</template>
