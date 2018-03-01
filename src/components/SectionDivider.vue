<template>
  <section :style="{backgroundImage: 'url('+image+')'}">
    <div class="inner">
      <SectionHeader :description="description" :title="title"/>
    </div>
  </section>
</template>

<script>
import SectionHeader from "./SectionHeader";

export default {
  name: "SectionDivider",
  components: {
    SectionHeader
  },
  props: {
    description: {
      default: "Description",
      type: String
    },
    title: {
      default: "Title",
      type: String
    },
    image: {
      default: "image.jpg",
      type: String
    }
  }
};
</script>

<style scoped>
section {
  background-color: #000;
  color: #bfbfbf;
  background-size: cover;
  background-attachment: fixed;
  background-position: center;
  position: relative;
  padding: 6rem 0 4rem 0;
  display: block;
}
section:before {
  transition-delay: 1.25s;
  content: "";
  display: block;
  background-color: rgba(0, 0, 0, 0.95);
  height: 100%;
  left: 0;
  opacity: 0.75;
  position: absolute;
  top: 0;
  width: 100%;
  z-index: 1;
}
section>>>h2 {
  color: #ffffff;
}
section>>>p {
  color: #bfbfbf;
}
section>>>p:after {
  background-color: rgba(255, 255, 255, 0.5);
}
.inner {
  position: relative;
  z-index: 2;
}
</style>
