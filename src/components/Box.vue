<template>
  <div class="box">
    <div class="image fit">
      <img :src="image" alt="">
    </div>
    <div class="content">
      <SectionHeader :description="description" :title="title"/>
      <p id="content">{{ content }}</p>
      <footer class="align-center">
        <a :href="buttonUrl" class="button alt">{{ buttonText }}</a>
      </footer>
    </div>
  </div>
</template>

<script>
import SectionHeader from "./SectionHeader";

export default {
  name: "Box",
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
    },
    content: {
      default: "Content",
      type: String
    },
    buttonText: {
      default: "Button Text",
      type: String
    },
    buttonUrl: {
      default: "Button Url",
      type: String
    }
  }
};
</script>

<style scoped>
.box {
  width: 100%;
  max-width: 600px;
  margin: 0 auto;
  background-color: #ffffff;
}
.image.fit img {
  width: 100%;
}
.box .content {
  padding: 3rem;
}
.content>>>h2 {
  color: #000;
  margin-bottom: 2rem;
}
p#content {
  margin: 0 0 2rem 0;
  color: #a6a6a6;
  padding: 0;
  border: 0;
  font-size: 100%;
  font: inherit;
  vertical-align: baseline;
  text-align: left;
}
.button.alt {
  background-color: transparent;
  box-shadow: inset 0 0 0 2px rgba(0, 0, 0, 0.15);
  color: #000 !important;
  transition: background-color 0.2s ease-in-out, color 0.2s ease-in-out;
  border-radius: 2px;
  border: 0;
  cursor: pointer;
  display: inline-block;
  font-weight: 300;
  height: 2.85rem;
  line-height: 2.95rem;
  padding: 0 1.5rem;
  text-align: center;
  text-decoration: none;
  text-transform: uppercase;
  white-space: nowrap;
}
</style>
