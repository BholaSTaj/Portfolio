<template>
  <nav class="fixed top-0 w-full bg-white shadow-sm z-50">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex justify-between items-center h-16">
        <span class="text-xl font-bold">BST</span>
        
        <!-- Desktop Menu -->
        <div class="hidden md:flex space-x-8">
          <button @click="scrollToSection('about')" class="hover:text-blue-600 transition">About</button>
          <button @click="scrollToSection('projects')" class="hover:text-blue-600 transition">Projects</button>
          <button @click="scrollToSection('skills')" class="hover:text-blue-600 transition">Skills</button>
          <button @click="scrollToSection('contact')" class="hover:text-blue-600 transition">Contact</button>
        </div>

        <!-- Mobile Menu Button -->
        <button @click="isMenuOpen = !isMenuOpen" class="md:hidden">
          <svg v-if="!isMenuOpen" class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"/>
          </svg>
          <svg v-else class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"/>
          </svg>
        </button>
      </div>
    </div>

    <!-- Mobile Menu -->
    <div v-if="isMenuOpen" class="md:hidden bg-white border-t">
      <div class="px-4 py-3 space-y-3">
        <button @click="scrollToSection('about')" class="block w-full text-left py-2 hover:text-blue-600">About</button>
        <button @click="scrollToSection('projects')" class="block w-full text-left py-2 hover:text-blue-600">Projects</button>
        <button @click="scrollToSection('skills')" class="block w-full text-left py-2 hover:text-blue-600">Skills</button>
        <button @click="scrollToSection('contact')" class="block w-full text-left py-2 hover:text-blue-600">Contact</button>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Navbar',
  data() {
    return {
      isMenuOpen: false
    }
  },
  methods: {
    scrollToSection(id) {
      const element = document.getElementById(id);
      if (element) {
        element.scrollIntoView({ behavior: 'smooth' });
        this.isMenuOpen = false;
      }
    }
  }
}
</script>