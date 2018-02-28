<template>
  <header class="align-center">
    <p>{{description}}</p>
    <h2>{{title}}</h2>
  </header>
</template>

<script>
export default {
  name: "SectionHeader",
  props: {
    description: {
      default: "Description",
      type: String
    },
    title: {
      default: "Title",
      type: String
    }
  }
};
</script>

<style scoped>
header p {
  position: relative;
  color: #999999;
  margin: 0 auto;
  width: 80rem;
}
p {
  text-transform: uppercase;
  font-size: 0.75rem;
  font-weight: 300;
  margin: 0 0 0.5rem 0;
  padding: 0 0 1rem 0;
  letter-spacing: 0.25rem;
}
p:after {
  content: "";
  position: absolute;
  margin: auto;
  right: 0;
  bottom: 0;
  left: 0;
  width: 50%;
  height: 1px;
  background-color: rgba(0, 0, 0, 0.125);
}
h2 {
  color: #555;
  font-size: 1.75rem;
  font-weight: 300;
  line-height: 1.5;
  margin: 0 0 1rem 0;
}
</style>
