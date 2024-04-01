<template>
  <!-- <button @click="show = !show">Menu</button> -->
  <Transition name="fade">
    <Header/>
  </Transition>
  <Productos/>
  <Cursos/>
  <Blog/>
  <Footer/>
</template>

<script>

import '../src/css/normalize.css'
import '../src/css/app.css'
import Header from './components/Header.vue';
import Productos from './components/Productos.vue';
import Cursos from './components/Cursos.vue';
import Blog from './components/Blog.vue';
import Footer from './components/Footer.vue';




export default {
  name: 'App',
  components: {
    Header,
    Productos,
    Cursos,
    Blog,
    Footer
  },
  data() {
    return {
      show: false,
    }
  }
}
</script>


