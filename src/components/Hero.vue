<template>
  <section class="pt-32 pb-20 px-4 sm:px-6 lg:px-8">
    <div class="max-w-6xl mx-auto">
      <h1 class="text-4xl sm:text-5xl lg:text-6xl font-bold mb-4">
        Hi, I'm <span class="text-blue-600">Bhola Shankar Tajpuriya</span>
      </h1>
      <p class="text-xl sm:text-2xl text-gray-600 mb-8">
        Full Stack Developer | Problem Solver | Tech Enthusiast
      </p>
      <p class="text-lg text-gray-700 max-w-2xl mb-8">
        I create elegant solutions to complex problems. Passionate about building 
        user-friendly web applications with clean, efficient code.
      </p>
      <div class="flex gap-4">

        <a href="/public/bholasCV.pdf" download="BholaSTaj.pdf" 
           class="flex items-center gap-2 bg-blue-500 border border-gray-300 px-6 py-3 rounded-lg hover:border-blue-600 hover:bg-blue-50 transition">
          <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 10v6m0 0l-3-3m3 3l3-3m2 8H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"/>
          </svg>
          Download CV
        </a>
        <a href="#projects" class="border border-gray-300 px-6 py-3 rounded-lg hover:border-blue-600 transition">
          View Work
        </a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Hero'
}
</script>