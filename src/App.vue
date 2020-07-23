<template>
  <div>
    <div class="app-container">
      <div class="container-side-images">
        <img src="../src/assets/gosia-left.png" alt="" />
      </div>
      <div id="app">
        <LocaleSwitcher />
        <Header />
        <div class="content-container">
          <AboutMe />
          <Languages />
        </div>
          <HowIWork />
          <Contact />
      </div>
      <div class="container-side-images">
        <img src="../src/assets/gosia-right.png" alt="" />
      </div>
    </div>
    <footer class="footer">website developed with ♡ by <a href="https://chiaradiaz.com" target="_blank">Chiara Diaz.</a></footer>
  </div>
</template>

<script>
import LocaleSwitcher from "./components/LocaleSwitcher/LocaleSwitcher";
import Header from "./components/Header/Header";
import AboutMe from "./components/AboutMe/AboutMe";
import HowIWork from "./components/HowIWork/HowIWork";
import Languages from "./components/Lan/Languages";
import Contact from "./components/Contact/Contact";
export default {
  name: "App",
  components: {
    LocaleSwitcher,
    Header,
    AboutMe,
    HowIWork,
    Languages,
    Contact
  }
};
</script>

<style>
body {
  margin: 0;
  padding: 0;
  background-color: #f7eee7;
}
.container-side-images {
  display: none;
}
.footer {
  text-align: center;
  font-family:  'futura std';
  font-size: 15px;
  color: #B3847C;
  margin-bottom: 20px;
}
a {
  text-decoration: none;
}
a:visited {
  color: #B3847C;
}
a:hover {
  color: #325147;
}
a:active {
  color: #B3847C;
}
</style>
