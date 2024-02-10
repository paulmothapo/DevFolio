<script setup>
const menuitems = [
 
  {
    title: "Portfolio",
    path: "/portfolio",
  },
  {
    title: "About",
    path: "/about",
  },
  {
    title: "Contact me",
    path: "/contact",
  },
  {
    title: "Resume",
    path: "/resume",
  },
];

const open = ref(false);
</script>

<template>
  <LandingContainer>
    <header class="flex flex-col lg:flex-row justify-between items-center  p-6 md:px-24">
      <div class="flex w-full lg:w-auto items-center justify-between">
        <a href="/" class="text-2xl"
          ><span class="font-bold text-slate-800">Dev</span
          ><span class="text-slate-500">Folio</span>
        </a>
        <div class="block lg:hidden">
          <button @click="open = !open" class="text-black">
            <svg
              fill="currentColor"
              class="w-4 h-4"
              viewBox="0 0 20 20"
              xmlns="http://www.w3.org/2000/svg"
            >
              <title>Menu</title>
              <path
                v-show="open"
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M18.278 16.864a1 1 0 01-1.414 1.414l-4.829-4.828-4.828 4.828a1 1 0 01-1.414-1.414l4.828-4.829-4.828-4.828a1 1 0 011.414-1.414l4.829 4.828 4.828-4.828a1 1 0 111.414 1.414l-4.828 4.829 4.828 4.828z"
              ></path>
              <path
                v-show="!open"
                fill-rule="evenodd"
                d="M4 5h16a1 1 0 010 2H4a1 1 0 110-2zm0 6h16a1 1 0 010 2H4a1 1 0 010-2zm0 6h16a1 1 0 010 2H4a1 1 0 010-2z"
              ></path>
            </svg>
          </button>
        </div>
      </div>
      <nav
        class="w-full lg:w-auto mt-2 lg:flex lg:mt-0"
        :class="{ block: open, hidden: !open }"
      >
        <ul class="flex flex-col lg:flex-row lg:gap-3">
          <li v-for="item of menuitems">
            <a
              :href="item.path"
              class="transition-transform transform flex lg:px-3 py-2 text-black hover:text-white border-b-4 border-b-red-500 hover:bg-red-500 hover:rounded-full font-semibold text-lg"
            >
              {{ item.title }}
            </a>
          </li>
        </ul>
      </nav>
    </header>
  </LandingContainer>
</template>
