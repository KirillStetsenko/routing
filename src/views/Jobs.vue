<template>
  <h1>Jobs</h1>
  <div v-for="job in jobs" :key="job.id" class="job">
    <h2>
      <router-link :to="{ name: 'JobDetails', params: { id: job.id } }">
        {{ job.title }}
      </router-link>
    </h2>
  </div>
</template>

<script>
export default {
  data() {
    return {
      jobs: [
        {
          id: 1,
          title: "React developer",
          salary: "1000$",
        },
        {
          id: 2,
          title: "Vue developer",
          salary: "2000$",
        },
        {
          id: 3,
          title: "Angular developer",
          salary: "3000$",
        },
      ],
    };
  },
};
</script>

<style>
.job h2 {
  margin: 10px auto;
  padding: 20px;
  max-width: 500px;
  border-radius: 20px;
  color: #444;
}

.job h2:hover {
  background: #aaa;
}

.job a {
  color: #444;
  text-decoration: none;
}
</style>
