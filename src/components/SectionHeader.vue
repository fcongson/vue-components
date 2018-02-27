<template>
  <header class="align-center">
    <p>{{description}}</p>
    <h2>{{title}}</h2>
  </header>
</template>

<script>
export default {
  name: "SectionHeader",
  props: ["description", "title"],
  data() {
    return {
      description: "Description",
      title: "Title"
    };
  }
};
</script>

<style scoped />;
