<template>
  <section id="skills" class="py-20 px-4 sm:px-6 lg:px-8 bg-gray-50">
    <div class="max-w-6xl mx-auto">
      <h2 class="text-3xl sm:text-4xl font-bold mb-8">Skills</h2>
      <div class="flex flex-wrap gap-3">
        <span v-for="(skill, index) in skills" :key="index" 
              class="bg-white border border-gray-200 px-4 py-2 rounded-lg text-gray-700 hover:border-blue-600 transition">
          {{ skill }}
        </span>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Skills',
  data() {
    return {
      skills: [
        "JavaScript", "Vue.js", "React", "Node.js", 
        "Tailwind CSS", "Git", "REST APIs", "MongoDB", "Express.js",
      ]
    }
  }
}
</script>