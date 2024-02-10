<script setup>
const projects = [
  {
    title: "Project 1",
    description: "Description of Project 1",
    languages: ["JavaScript", "HTML", "CSS"],
  },
  {
    title: "Project 2",
    description: "Description of Project 2",
    languages: ["Python", "Django", "JavaScript"],
  },
];
</script>

<template>
  <div class="mt-16 md:mt-0">
    <h2 class="text-4xl lg:text-5xl font-bold lg:tracking-tight">
      Featured Projects
    </h2>
    <p class="text-lg mt-4 text-slate-600">
      Check out some of my featured projects and the programming languages used.
    </p>
  </div>

  <div class="grid sm:grid-cols-2 md:grid-cols-3 mt-16 gap-16">
    <div v-for="project of projects" class="flex gap-4 items-start">
      <div class="mt-1 bg-black rounded-full p-2 w-8 h-8 shrink-0">
        <Icon class="text-white" name="bx:bxs-briefcase" />
      </div>
      <div>
        <h3 class="font-semibold text-lg">{{ project.title }}</h3>
        <p class="text-slate-500 mt-2 leading-relaxed">
          {{ project.description }}
          <br />
          <strong>Languages used:</strong> {{ project.languages.join(", ") }}
        </p>
      </div>
    </div>
  </div>
</template>
