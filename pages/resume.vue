<script setup>
definePageMeta({
  layout: "landing",
});

</script>

<template>
    <LandingContainer>
      <div class="flex flex-col min-h-screen items-center justify-center md:px-20 px-16 ">
        <h1 class="text-3xl font-bold text-gray-800 mb-8 ">My Resume</h1>
        <p class="text-lg text-gray-800 mb-8 mt-8">
          As a skilled Full Stack Developer with extensive experience in building web applications, I bring a unique blend of technical expertise and creative problem-solving skills to every project. Let my passion for coding and dedication to excellence help you achieve your goals.
        </p>
        <a href="/JohnWick.pdf" type="application/pdf" download class="mt-10 hover:text-red-500 text-black border-b-4 border-b-red-500 font-bold py-2 px-4 rounded transition duration-300">
          Download Resume (PDF)
        </a>
      </div>
    </LandingContainer>
  </template>
  

  