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
    <h2>usage</h2>
    <pre><code>&lt;SectionHeader description="Nam vel ante sit amet libero scelerisque facilisis eleifend vitae urna" title="Morbi maximus justo" image="url(./assets/images/bg.jpg)"/&gt;</code></pre>
    <h2>preview</h2>
    <div class="component-preview">
    <SectionDivider description="Nam vel ante sit amet libero scelerisque facilisis eleifend vitae urna" title="Morbi maximus justo" image="url(./assets/images/bg.jpg)"/>
    </div>
    </div>
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld";
import SectionHeader from "./components/SectionHeader";
import SectionDivider from "./components/SectionDivider";

export default {
  name: "App",
  components: {
    // HelloWorld,
    SectionHeader,
    SectionDivider
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
.component-section {
  margin: 40px 0px 40px 0px;
}
.component-preview {
  border-style: solid;
  border-width: 1px;
  border-color: #eeeeee;
}
</style>
