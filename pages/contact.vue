<script setup>
definePageMeta({
  layout: "landing",
});
</script>

<template>
  <LandingContainer>
    <LandingSectionhead>
      <template v-slot:title>Contact Me</template>
      <template v-slot:desc>This is the part where we collaborate. I am here for you.</template>
    </LandingSectionhead>

    <div class="grid md:grid-cols-2 gap-10 md:mx-auto mx-10 md:max-w-4xl mt-16">
      <div>
        <h2 class="font-medium text-2xl text-gray-800">
          Contact John Wick
        </h2>
        <p class="text-lg leading-relaxed text-gray-800 mt-3">
          I'm your go-to Full Stack Developer! Whether you need assistance with a project or have a question, feel free to reach out by filling out the form below or sending me an email. And don't worry, I'm a quick replier!
        </p>
        <div class="mt-5">
          <div class="flex items-center mt-2 space-x-2 text-gray-600">
            <Icon class="text-gray-400 w-4 h-4" name="uil:map-marker" />
            <span>Mars, south B3, Section 44</span>
          </div>
          <div class="flex items-center mt-2 space-x-2 text-gray-600">
            <Icon class="text-gray-400 w-4 h-4" name="uil:envelope" /><a
              href="mailto:jakobaichmayr@gmail.com"
              >johnwick@DevFolio.com</a
            >
          </div>
        </div>
      </div>
      <div>
        <LandingContactform />
      </div>
    </div>
  </LandingContainer>
</template>
