<template>
  <footer class="my-20 bg-black py-16">
    <div class="flex justify-center mt-4 mb-6">
      <a
        href="https://twitter.com/your-twitter-handle"
        target="_blank"
        rel="noopener"
        class="mr-4"
      >
        <Icon class="text-white" name="bx:bxl-twitter" size="24" />
      </a>
      <a
        href="https://linkedin.com/in/your-linkedin-profile"
        target="_blank"
        rel="noopener"
        class="mr-4"
      >
        <Icon class="text-white" name="bx:bxl-linkedin" size="24" />
      </a>
      <a
        href="https://github.com/your-github-profile"
        target="_blank"
        rel="noopener"
        class="mr-4"
      >
        <Icon class="text-white" name="bx:bxl-github" size="24" />
      </a>
    </div>
    <p class="text-center text-sm text-white">
      Copyright © {{ new Date().getFullYear() }} DevFolio. All rights reserved.
    </p>
    <p class="text-center text-xs text-white mt-1">
      Made by
      <a
        href="https://github.com/paulmothapo"
        target="_blank"
        rel="noopener"
        class="hover:underline"
      >
        Paul Mothapo
      </a>
    </p>
    
  </footer>
</template>
