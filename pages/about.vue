<template>
  <LandingContainer>
    <LandingSectionhead>
      <template v-slot:title>About Me</template>
    </LandingSectionhead>

    <div class="flex flex-col md:flex-row gap-8 items-center mx-auto max-w-4xl mt-12 text-gray-800">
      <div class="md:w-1/2 w-96">
        <img src="~/assets/img/man.jpg" alt="John Wick" class="h-96 w-80 rounded-lg shadow-lg">
      </div>
      
      <div class="md:w-1/2 w-96">
        <h2 class="font-bold text-3xl">John Wick</h2>
        <p class="text-lg leading-relaxed mt-4 border-b-2 border-b-red-500">
          Full Stack Developer, UX Design, Pool Fanatic
        </p>
        <p class="text-lg text-gray-800 leading-relaxed mt-4">
          Two years ago, I embarked on a journey with no prior coding experience. Despite being a high school graduate without university education, I was determined to learn and grow in the field of software development. Through constant learning and seizing the opportunity to join the WeThinkCode program, I started gaining valuable coding experience.
        </p>
        <p class="text-lg text-gray-800 leading-relaxed mt-4">
          I immersed myself in various programming languages such as Python and Java, and even dabbled in using APIs like Google Calendar. Surprisingly, I found myself excelling in coding, often jokingly saying that I can code better than university graduates. It's been an incredible journey filled with challenges and triumphs, and I'm excited for what lies ahead in my coding career.
        </p>
       
      </div>
    </div>
    <div class="mt-4 mb-6 items-center justify-center  mx-10 md:mx-auto md:max-w-4xl border-t-2">
      <h3 class="font-bold text-xl mt-8">Education</h3>
        <p class="text-lg text-gray-800 leading-relaxed mt-4">
          Wethink Code - 2024
        </p>

        <h3 class="font-bold text-xl mt-8">Skills</h3>
          <ul class="list-disc text-base text-gray-800 leading-relaxed mt-4 ml-8">
            <li><span class="font-bold text-lg">Languages:</span> JavaScript/TypeScript, Python, Java</li>
            <li><span class="font-bold text-lg">Frontend:</span> Vue.js, React, HTML/CSS, Tailwind CSS</li>
            <li><span class="font-bold text-lg">Backend:</span> Node.js, Express, Django, Flask</li>
            <li><span class="font-bold text-lg">Databases:</span> MongoDB, PostgreSQL, MySQL</li>
            <li><span class="font-bold text-lg">Tools & Technologies:</span> Git, Docker, RESTful APIs, GraphQL</li>
            <li><span class="font-bold text-lg">UI/UX Design:</span> Figma, Adobe XD, Sketch</li>
          </ul>

        <h3 class="font-bold text-xl mt-8">Experience</h3>
        <div class="text-lg text-gray-800 leading-relaxed mt-4">
          <p class="border-b-2 border-b-red-500">Full Stack Developer | ABC Tech Solutions | 2022 - Present</p>
          <ul class="list-disc pl-8 text-base">
            <li>Led the development of a responsive website using Next.js and TypeScript, resulting in improved performance and user engagement.</li>
            <li>Designed and implemented a mobile app for scanning products in retail stores, streamlining inventory management processes and enhancing customer experience.</li>
            <li>Developed an API for Dev Folio to facilitate easy integration for recruiters, enabling seamless communication and data exchange.</li>
          </ul>
        </div>
    </div>
  </LandingContainer>
</template>
