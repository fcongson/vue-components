<template>
  <div id="app">
    <img src="./assets/logo.png">
    <!-- <HelloWorld/> -->

    <!-- Section Header -->
    <hr/>
    <div class="component-section">
      <h1>Section Header</h1>
      <p>Section header with customizable <code><b>title</b></code> and <code><b>description</b></code></p>
      <h2>usage</h2>
      <pre><code>&lt;SectionHeader description="Nam vel ante sit amet libero scelerisque facilisis eleifend vitae urna" title="Morbi maximus justo"/&gt;</code></pre>
      <h2>preview</h2>
      <div class="component-preview">
        <SectionHeader description="Nam vel ante sit amet libero scelerisque facilisis eleifend vitae urna" title="Morbi maximus justo"/>
      </div>
    </div>

    <!-- Section Divider -->
    <hr/>
    <div class="component-section">
      <h1>Section Divider</h1>
      <p>Section header with customizable <code><b>title</b></code>, <code><b>description</b></code>, and <code><b>image</b></code></p>
      <p><i>*note: the static path is needed when using images with webpack</i></p>
      <h2>usage</h2>
      <pre><code>&lt;SectionHeader description="Nam vel ante sit amet libero scelerisque facilisis eleifend vitae urna" title="Morbi maximus justo" image="./assets/images/bg.jpg"/&gt;</code></pre>
      <h2>preview</h2>
      <div class="component-preview">
        <SectionDivider description="Nam vel ante sit amet libero scelerisque facilisis eleifend vitae urna" title="Morbi maximus justo" :image="bgJpg"/>
      </div>
    </div>

    <!-- Box -->
    <hr/>
    <div class="component-section">
      <h1>Box</h1>
      <p>Box with customizable <code><b>title</b></code>, <code><b>description</b></code>, <code><b>image</b></code>, <code><b>content</b></code>, <code><b>buttonText</b></code>, and <code><b>buttonUrl</b></code></p>
      <p><i>*note: the static path is needed when using images with webpack</i></p>
      <h2>usage</h2>
      <pre><code>&lt;Box description="maecenas sapien feugiat ex purus" title="Lorem ipsum dolor" image="./assets/images/pic02.jpg" content="Cras aliquet urna ut sapien tincidunt, quis malesuada elit facilisis. Vestibulum sit amet tortor velit. Nam elementum nibh a libero pharetra elementum. Maecenas feugiat ex purus, quis volutpat lacus placerat malesuada." buttonText="Learn More" buttonUrl="#"/&gt;</code></pre>
      <h2>preview</h2>
      <div class="component-preview dark">
        <Box description="maecenas sapien feugiat ex purus" title="Lorem ipsum dolor" :image="pic02" content="Cras aliquet urna ut sapien tincidunt, quis malesuada elit facilisis. Vestibulum sit amet tortor velit. Nam elementum nibh a libero pharetra elementum. Maecenas feugiat ex purus, quis volutpat lacus placerat malesuada." buttonText="Learn More" buttonUrl="#"/>
      </div>
    </div>

  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld";
import SectionHeader from "./components/SectionHeader";
import SectionDivider from "./components/SectionDivider";
import Box from "./components/Box";

// asset images
import bgJpg from "./assets/images/bg.jpg";
import pic02 from "./assets/images/pic02.jpg";

export default {
  name: "App",
  components: {
    // HelloWorld,
    SectionHeader,
    SectionDivider,
    Box
  },
  data() {
    return {
      bgJpg: bgJpg,
      pic02: pic02
    };
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
h1,
h2 {
  font-weight: normal;
}
pre {
  padding: 20px;
  background: #eeeeee;
  overflow: auto;
}
.component-section {
  margin: 40px 0px 40px 0px;
}
.component-preview {
  border-style: solid;
  border-width: 1px;
  border-color: #eeeeee;
}
.component-preview.dark {
  background-color: #eeeeee;
}
</style>
