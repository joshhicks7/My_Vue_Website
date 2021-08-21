<template>
  <div class="app">
    <Header />
    <div class = "app_body">
      <AboutMe />
      <Project_Container />
      <Contact/>
    </div>   
    <div class = "footer"></div>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Project_Container from "./components/Project_Container.vue";
import AboutMe from "./components/AboutMe.vue"
import Contact from './components/Contact.vue'
export default {
  name: "App",
  components: {
    Header,
    Project_Container,
    AboutMe,
    Contact
  },
};
</script>

<style>
.app {
  display: flex;
  flex-direction: column;
  margin:0px;
}
.app_body
{  
  background-image:linear-gradient(to bottom, black, blue, purple); 
  background-repeat: no-repeat;
}
</style>
