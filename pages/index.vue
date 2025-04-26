<template>
  <div>
    <!-- Hero Section -->
    <section class="relative bg-white dark:bg-gray-800 overflow-hidden">
      <div class="max-w-7xl mx-auto">
        <div class="relative z-10 pb-8 bg-white dark:bg-gray-800 sm:pb-16 md:pb-20 lg:max-w-2xl lg:w-full lg:pb-28 xl:pb-32">
          <main class="mt-10 mx-auto max-w-7xl px-4 sm:mt-12 sm:px-6 md:mt-16 lg:mt-20 lg:px-8 xl:mt-28">
            <div class="sm:text-center lg:text-left">
              <h1 class="text-4xl tracking-tight font-extrabold text-gray-900 dark:text-white sm:text-5xl md:text-6xl">
                <span class="block">Hallo, ik ben</span>
                <span class="block text-blue-600 dark:text-blue-500">Mehmet Furkan</span>
              </h1>
              <p class="mt-3 text-base text-gray-500 dark:text-gray-400 sm:mt-5 sm:text-lg sm:max-w-xl sm:mx-auto md:mt-5 md:text-xl lg:mx-0">
                Full Stack Developer met een passie voor het creëren van innovatieve oplossingen. Momenteel in mijn laatste jaar aan Hogeschool PXL, met specialisatie in Applicatieontwikkeling.
              </p>
              <div class="mt-5 sm:mt-8 sm:flex sm:justify-center lg:justify-start">
                <div class="rounded-md shadow">
                  <NuxtLink to="/projects" class="w-full flex items-center justify-center px-8 py-3 border border-transparent text-base font-medium rounded-md text-white bg-blue-600 hover:bg-blue-700 md:py-4 md:text-lg md:px-10">
                    Bekijk Projecten
                  </NuxtLink>
                </div>
                <div class="mt-3 sm:mt-0 sm:ml-3">
                  <NuxtLink to="/about" class="w-full flex items-center justify-center px-8 py-3 border border-transparent text-base font-medium rounded-md text-blue-700 bg-blue-100 hover:bg-blue-200 md:py-4 md:text-lg md:px-10">
                    Over Mij
                  </NuxtLink>
                </div>
              </div>
            </div>
          </main>
        </div>
      </div>
    </section>

    <!-- Featured Activities -->
    <section class="py-12 bg-gray-50 dark:bg-gray-900">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="lg:text-center">
          <h2 class="text-3xl font-extrabold tracking-tight text-gray-900 dark:text-white sm:text-4xl">
            Uitgelichte Activiteiten
          </h2>
          <p class="mt-4 max-w-2xl text-xl text-gray-500 dark:text-gray-400 lg:mx-auto">
            Ontdek mijn reis door verschillende activiteiten en ervaringen.
          </p>
        </div>

        <div class="mt-10">
          <div class="space-y-10 md:space-y-0 md:grid md:grid-cols-2 md:gap-x-8 md:gap-y-10">
            <!-- Project Week Card -->
            <div class="relative">
              <div class="bg-white dark:bg-gray-800 p-6 rounded-lg shadow-lg">
                <h3 class="text-lg font-medium text-gray-900 dark:text-white">Projectweek 2TIN</h3>
                <p class="mt-2 text-base text-gray-500 dark:text-gray-400">
                  Intensieve week gericht op persoonlijke en professionele ontwikkeling door middel van workshops en teamactiviteiten.
                </p>
                <NuxtLink to="/projects#project-week" class="mt-3 inline-flex items-center text-blue-600 hover:text-blue-500">
                  Lees meer
                  <svg class="ml-2 w-5 h-5" fill="currentColor" viewBox="0 0 20 20">
                    <path fill-rule="evenodd" d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z" clip-rule="evenodd" />
                  </svg>
                </NuxtLink>
              </div>
            </div>

            <!-- Hackathon Card -->
            <div class="relative">
              <div class="bg-white dark:bg-gray-800 p-6 rounded-lg shadow-lg">
                <h3 class="text-lg font-medium text-gray-900 dark:text-white">Hack The Future 2024</h3>
                <p class="mt-2 text-base text-gray-500 dark:text-gray-400">
                  Deelgenomen aan de Flexso Challenge, waarbij we een webapplicatie ontwikkelden met SAP-technologieën.
                </p>
                <NuxtLink to="/projects#hackathon" class="mt-3 inline-flex items-center text-blue-600 hover:text-blue-500">
                  Lees meer
                  <svg class="ml-2 w-5 h-5" fill="currentColor" viewBox="0 0 20 20">
                    <path fill-rule="evenodd" d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z" clip-rule="evenodd" />
                  </svg>
                </NuxtLink>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template> 