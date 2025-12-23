<template>
  <section id="projects" class="py-20 px-4 sm:px-6 lg:px-8">
    <div class="max-w-6xl mx-auto">
      <h2 class="text-3xl sm:text-4xl font-bold mb-8">Projects</h2>
      <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-6">
        <div v-for="(project, index) in projects" :key="index" 
             class="bg-white border border-gray-200 rounded-lg p-6 hover:shadow-lg transition">
          <h3 class="text-xl font-semibold mb-2">{{ project.title }}</h3>
          <p class="text-gray-600 mb-4">{{ project.description }}</p>
          <div class="flex flex-wrap gap-2 mb-4">
            <span v-for="(tag, i) in project.tags" :key="i" 
                  class="bg-blue-100 text-blue-600 text-sm px-3 py-1 rounded">
              {{ tag }}
            </span>
          </div>
          <a :href="project.link" class="inline-flex items-center text-blue-600 hover:text-blue-700">
            View Project
            <svg class="w-4 h-4 ml-1" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 6H6a2 2 0 00-2 2v10a2 2 0 002 2h10a2 2 0 002-2v-4M14 4h6m0 0v6m0-6L10 14"/>
            </svg>
          </a>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Projects',
  data() {
    return {
      projects: [
        {
          title: "Project One: Service Friend",
          description: "A web-based platform that bridges the gap between local service seekers and providers    through a centralized and intuitive system.",
          tags: ["NodeJS", "MongoDB", "Tailwind CSS"],
          link: "https://servicefriend.vercel.app/"
        },
        {
          title: "Project Two: Quote Generator",
          description: "A web application built to generate in-built quotes.",
          tags: ["Vue.js"],
          link: "https://quote-generator-kappa-two.vercel.app/"
          
        },
        {
          title: "Project Three: Ecommerce clone",
          description: "Developed a fully responsive e-commerce homepage using HTML, CSS, and Font Awesome to replicate modern online shopping UI patterns.",
          tags: ["CSS", "JavaScript", "Figma"],
          link: "https://ecommerce-nu-blond.vercel.app/"
        }
      ]
    }
  }
}
</script>