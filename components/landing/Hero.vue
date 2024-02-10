<template>
  <main class="grid lg:grid-cols-2 place-items-center md:pt-8">
    <div class="md:p-24 md:order-1 mx-36">
      <img
        class="rounded-full transition-transform transform hover:scale-120"
        src="~/assets/img/man.jpg"
        alt="Starship starts the engine"
        loading="eager"
        format="avif"
        width="512"
        height="512"
      />
    </div>

    <div class="p-10">
      <h1 class="text-5xl lg:text-6xl xl:text-7xl font-bold lg:tracking-tight">
        John Wick
      </h1>
      <p class="text-lg mt-4 text-black max-w-xl">
        I am a proficient software engineer with over 2 years of coding experience. Known for my dedication and hard work, I thrive in challenging environments and continuously strive for excellence. With a strong foundation in various programming languages and technologies, I am passionate about solving complex problems and delivering high-quality solutions. Read more <a href="/about" class="underline font-bold">about me</a> and explore <a href="/portfolio" class="underline font-bold">my projects</a>.
      </p>

      <div class="mt-6 flex flex-col sm:flex-row gap-3 text-gray-500">
        <div
          
          >DevFolio developed by <a 
          class="font-semibold text-red-700 italic"
          href="https://github.com/paulmothapo"
          target="_blank"
          rel="noopener"
          >paulmothapo</a></div
        >
      </div>
    </div>
  </main>
</template>
