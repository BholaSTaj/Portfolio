<script>
import Navbar from './components/Navbar.vue'
import Hero from './components/Hero.vue'
import About from './components/About.vue'
import Projects from './components/Projects.vue'
import Skills from './components/Skills.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    Hero,
    About,
    Projects,
    Skills,
    Contact,
    Footer
  }
}
</script>

<template>
  <div class="min-h-screen bg-white text-gray-900">
    <Navbar />
    <Hero />
    <About />
    <Projects />
    <Skills />
    <Contact />
    <Footer></Footer>
  </div>
</template>