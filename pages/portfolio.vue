<script setup>
definePageMeta({
  layout: "landing",
});

const projects = [
  {
    title: "E-commerce Website with Next.js",
    description: "Developed a full-fledged e-commerce platform using Next.js, incorporating TypeScript for enhanced type checking and code maintainability. Implemented features such as product listings, user authentication, and checkout functionality.",
    technologies: "Next.js, TypeScript, Tailwind CSS, MongoDB"
  },
  {
    title: "Retail Product Scanner App",
    description: "Designed and built a mobile application for scanning products in retail stores, allowing users to view product details and check availability in real-time. Integrated with backend APIs to fetch and update product information from the database.",
    technologies: "React Native, Node.js, Express, MongoDB"
  },
  {
    title: "Dev Folio Integration API",
    description: "Created an API for Dev Folio to facilitate seamless integration with recruiting platforms, allowing recruiters to access and manage candidate data more efficiently. Implemented authentication and authorization mechanisms to ensure data security and privacy.",
    technologies: "Node.js, Express, MongoDB, JWT"
  }
];

const certifications = [
  "AWS Certified Developer - Associate",
  "Google Certified Professional - Cloud Architect"
];
</script>

<template>
  <LandingContainer>
    <LandingSectionhead>
      <template v-slot:title>Portfolio</template>
      <template v-slot:desc>Explore my projects and certifications.</template>
    </LandingSectionhead>

    <div class="flex flex-col gap-8 md:mx-auto mx-12 max-w-4xl mt-16">
      <h2 class="font-bold text-3xl text-gray-800 border-b-2 border-b-red-600 ">Projects</h2>
      <div v-for="(project, index) in projects" :key="index" class="mt-6">
        <h3 class="font-semibold text-xl text-gray-800">{{ project.title }}</h3>
        <p class="text-gray-600 mt-2">{{ project.description }}</p>
        <p class=" mt-2 font-bold text-red-600"><span class="text-gray-800 font-normal">Technologies Used:</span> {{ project.technologies }}</p>
      </div>
      
      <h2 class="font-bold text-3xl text-gray-800 mt-12 border-b-2 border-b-red-600 ">Certifications</h2>
      <ul class="list-disc list-inside text-gray-600 mt-4 mb-12">
        <li v-for="(certification, index) in certifications" :key="index">{{ certification }}</li>
      </ul>
    </div>
  
  </LandingContainer>
</template>
