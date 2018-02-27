<template>
  <div id="app">
    <img src="./assets/logo.png">
    <!-- <HelloWorld/> -->
    <hr/>
    <h1>Section Header</h1>
    <p>Section header with customizable <code><b>title</b></code> and <code><b>description</b></code></p>
    <h2>usage</h2>
    <pre><code>&lt;SectionHeader description="Nam vel ante sit amet libero scelerisque facilisis eleifend vitae urna" title="Morbi maximus justo"/&gt;</code></pre>
    <h2>preview</h2>
    <div class="component-preview">
    <SectionHeader description="Nam vel ante sit amet libero scelerisque facilisis eleifend vitae urna" title="Morbi maximus justo"/>
    </div>
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld";
import SectionHeader from "./components/SectionHeader";

export default {
  name: "App",
  components: {
    // HelloWorld,
    SectionHeader
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
}
.component-preview {
  border-style: solid;
  border-width: 1px;
  border-color: #eeeeee;
}
</style>
