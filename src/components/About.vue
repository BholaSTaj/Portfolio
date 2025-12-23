<template>
  <section id="about" class="py-20 px-4 sm:px-6 lg:px-8 bg-gray-50">
    <div class="max-w-6xl mx-auto">
      <h2 class="text-3xl sm:text-4xl font-bold mb-8">About Me</h2>
      <div class="grid md:grid-cols-2 gap-8">
        <div>
          <p class="text-gray-700 mb-4">
            I'm a passionate developer with a focus on creating intuitive and efficient 
            web applications. With experience in modern frameworks and technologies, 
            I bring ideas to life through code.
          </p>
          <p class="text-gray-700">
            When I'm not coding, you can find me exploring new technologies, contributing 
            to open-source projects, or sharing knowledge with the developer community.
          </p>
        </div>
        <div class="bg-white p-6 rounded-lg shadow-sm">
          <h3 class="font-semibold text-xl mb-4">Quick Facts</h3>
          <ul class="space-y-2 text-gray-700">
            <li>📍 Location: Kathmandu, Nepal</li>
            <li>🎓 Education: Currently pursuing BSc.Csit</li>
            <!-- <li>💼 Experience: Workshops Attended</li> -->
            <li>🌐 Languages: English,Nepali</li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'About'
}
</script>