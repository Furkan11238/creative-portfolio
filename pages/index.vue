<template>
  <div class="min-h-screen bg-gradient-to-br from-white to-primary-50/30 dark:from-gray-900 dark:to-primary-900/30">
    <!-- Hero Section -->
    <div class="relative py-24 overflow-hidden">
      <div class="absolute inset-0 bg-gradient-to-b from-primary-500/10 to-transparent dark:from-primary-500/5"></div>
      <div class="relative max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="lg:grid lg:grid-cols-12 lg:gap-8">
          <div class="sm:text-center md:max-w-2xl md:mx-auto lg:col-span-6 lg:text-left">
            <h1 class="text-4xl tracking-tight font-extrabold text-gray-900 dark:text-white sm:text-5xl md:text-6xl animate-fade-in">
              <span class="block">Hallo, ik ben</span>
              <span class="block text-primary-600 dark:text-primary-400">Mehmet Furkan</span>
            </h1>
            <p class="mt-3 text-base text-gray-500 dark:text-gray-400 sm:mt-5 sm:text-lg sm:max-w-xl sm:mx-auto md:mt-5 md:text-xl lg:mx-0 animate-slide-in">
              Full Stack Developer met een passie voor het creëren van innovatieve oplossingen. Momenteel in mijn laatste jaar aan Hogeschool PXL, met specialisatie in Applicatieontwikkeling.
            </p>
            <div class="mt-5 sm:mt-8 sm:flex sm:justify-center lg:justify-start">
              <div class="rounded-md shadow">
                <NuxtLink to="/projects" class="w-full flex items-center justify-center px-8 py-3 border border-transparent text-base font-medium rounded-md text-white bg-primary-600 hover:bg-primary-700 md:py-4 md:text-lg md:px-10 transition-colors">
                  Bekijk Projecten
                </NuxtLink>
              </div>
              <div class="mt-3 sm:mt-0 sm:ml-3">
                <NuxtLink to="/about" class="w-full flex items-center justify-center px-8 py-3 border border-transparent text-base font-medium rounded-md text-primary-700 bg-primary-100 hover:bg-primary-200 md:py-4 md:text-lg md:px-10 transition-colors">
                  Over Mij
                </NuxtLink>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Featured Activities -->
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 pb-24">
      <div class="text-center mb-12">
        <h2 class="text-3xl font-bold text-gray-900 dark:text-white mb-4">
          Uitgelichte Activiteiten
        </h2>
        <p class="text-xl text-gray-600 dark:text-gray-300 max-w-3xl mx-auto">
          Ontdek mijn reis door verschillende activiteiten en ervaringen
        </p>
      </div>

      <div class="grid gap-8 md:grid-cols-2">
        <!-- Project Week Card -->
        <div class="bg-white dark:bg-gray-800 rounded-2xl shadow-sm hover:shadow-xl transition-all duration-300 overflow-hidden border border-gray-100 dark:border-gray-700 group">
          <div class="p-6">
            <div class="flex items-center justify-between mb-4">
              <h3 class="text-lg font-semibold text-gray-900 dark:text-white group-hover:text-primary-500 dark:group-hover:text-primary-400 transition-colors">
                Projectweek 2TIN
              </h3>
              <span class="flex items-center justify-center w-10 h-10 rounded-full bg-primary-50 dark:bg-primary-900/50 group-hover:bg-primary-100 dark:group-hover:bg-primary-800/50 transition-colors">
                <svg class="w-5 h-5 text-primary-500 dark:text-primary-400" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 11H5m14 0a2 2 0 012 2v6a2 2 0 01-2 2H5a2 2 0 01-2-2v-6a2 2 0 012-2m14 0V9a2 2 0 00-2-2M5 11V9a2 2 0 012-2m0 0V5a2 2 0 012-2h6a2 2 0 012 2v2M7 7h10" />
                </svg>
              </span>
            </div>
            <p class="text-gray-600 dark:text-gray-300 text-sm">
              Intensieve week gericht op persoonlijke en professionele ontwikkeling door middel van workshops en teamactiviteiten.
            </p>
            <div class="mt-4 pt-4 border-t border-gray-100 dark:border-gray-700">
              <NuxtLink to="/projects#project-week" class="inline-flex items-center text-primary-600 hover:text-primary-500 dark:text-primary-400 dark:hover:text-primary-300">
                Lees meer
                <svg class="ml-2 w-5 h-5" fill="currentColor" viewBox="0 0 20 20">
                  <path fill-rule="evenodd" d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z" clip-rule="evenodd" />
                </svg>
              </NuxtLink>
            </div>
          </div>
        </div>

        <!-- Hackathon Card -->
        <div class="bg-white dark:bg-gray-800 rounded-2xl shadow-sm hover:shadow-xl transition-all duration-300 overflow-hidden border border-gray-100 dark:border-gray-700 group">
          <div class="p-6">
            <div class="flex items-center justify-between mb-4">
              <h3 class="text-lg font-semibold text-gray-900 dark:text-white group-hover:text-accent-500 dark:group-hover:text-accent-400 transition-colors">
                Hack The Future 2024
              </h3>
              <span class="flex items-center justify-center w-10 h-10 rounded-full bg-accent-50 dark:bg-accent-900/50 group-hover:bg-accent-100 dark:group-hover:bg-accent-800/50 transition-colors">
                <svg class="w-5 h-5 text-accent-500 dark:text-accent-400" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z" />
                </svg>
              </span>
            </div>
            <p class="text-gray-600 dark:text-gray-300 text-sm">
              Deelgenomen aan de Flexso Challenge, waarbij we een webapplicatie ontwikkelden met SAP-technologieën.
            </p>
            <div class="mt-4 pt-4 border-t border-gray-100 dark:border-gray-700">
              <NuxtLink to="/projects#hackathon" class="inline-flex items-center text-accent-600 hover:text-accent-500 dark:text-accent-400 dark:hover:text-accent-300">
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
  </div>
</template>

<style scoped>
.animate-fade-in {
  animation: fadeIn 1s ease-out;
}

.animate-slide-in {
  animation: slideIn 1s ease-out;
}

@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

@keyframes slideIn {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style> 