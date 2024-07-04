<template>
  <div class="jobDetails">
    <h1>Job Detail Page</h1>
    <p>Job id is {{ id }}</p>
  </div>
</template>

<script>
export default {
  //can use this
  props: ["id"], 
  
  // or this
  
  /* data() {
    return {
      id: this.$route.params.id,
    };
  }, */
};
</script>

<style></style>
