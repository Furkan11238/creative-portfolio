<template>
  <div class="min-h-screen bg-gradient-to-br from-white to-primary-50/30 dark:from-gray-900 dark:to-primary-900/30">
    <!-- Header -->
    <div class="relative py-24 overflow-hidden">
      <div class="absolute inset-0 bg-gradient-to-b from-primary-500/10 to-transparent dark:from-primary-500/5"></div>
      <div class="relative max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
        <h1 class="text-4xl md:text-5xl font-bold text-gray-900 dark:text-white text-center mb-4 animate-fade-in">
          Over Mij
        </h1>
        <p class="text-xl text-gray-600 dark:text-gray-300 text-center max-w-3xl mx-auto animate-slide-in">
          Een gepassioneerde full-stack developer met focus op het creëren van innovatieve oplossingen
        </p>
      </div>
    </div>

    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 pb-24">
      <!-- Personal Info -->
      <div class="bg-white dark:bg-gray-800 rounded-2xl shadow-sm hover:shadow-xl transition-all duration-300 overflow-hidden border border-gray-100 dark:border-gray-700 group mb-12">
        <div class="p-6">
          <div class="flex items-center justify-between mb-4">
            <h2 class="text-xl font-semibold text-gray-900 dark:text-white group-hover:text-primary-500 dark:group-hover:text-primary-400 transition-colors">
              Persoonlijke Informatie
            </h2>
            <span class="flex items-center justify-center w-10 h-10 rounded-full bg-primary-50 dark:bg-primary-900/50 group-hover:bg-primary-100 dark:group-hover:bg-primary-800/50 transition-colors">
              <svg class="w-6 h-6 text-primary-500 dark:text-primary-400" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z" />
              </svg>
            </span>
          </div>
          <div class="space-y-4 text-gray-600 dark:text-gray-300">
            <p>
              Mijn naam is Mehmet Karakoc, ik ben 22 jaar en momenteel zit ik in mijn laatste jaar aan Hogeschool PXL, 
              richting Toegepaste Informatica met als afstudeerrichting Applicatieontwikkeling. Ik ben een rustige en 
              behulpzame persoon die graag anderen ondersteunt wanneer nodig. Betrouwbaarheid, loyaliteit en zelfstandig 
              werken zijn eigenschappen die goed bij mij passen.
            </p>
            <p>
              In mijn vrije tijd hou ik mij graag bezig met gaming, muziek beluisteren, reizen en het spelen van 
              basketbal of voetbal. Deze hobby's zorgen ervoor dat ik een goed evenwicht vind tussen werk en ontspanning.
            </p>
            <p>
              Als fullstack developer heb ik een brede interesse in zowel frontend, backend als mobile development. 
              Ik werk graag met verschillende technologieën en frameworks, omdat ik het belangrijk vind om mij continu 
              verder te ontwikkelen binnen IT. Mijn grootste talent als developer is probleemoplossend denken en het 
              nauwkeurig afwerken van projecten.
            </p>
          </div>
        </div>
      </div>

      <div class="grid gap-8 md:grid-cols-2">
        <!-- Technical Skills -->
        <div class="bg-white dark:bg-gray-800 rounded-2xl shadow-sm hover:shadow-xl transition-all duration-300 overflow-hidden border border-gray-100 dark:border-gray-700 group">
          <div class="p-6">
            <div class="flex items-center justify-between mb-4">
              <h2 class="text-xl font-semibold text-gray-900 dark:text-white group-hover:text-secondary-500 dark:group-hover:text-secondary-400 transition-colors">
                Technische Vaardigheden
              </h2>
              <span class="flex items-center justify-center w-10 h-10 rounded-full bg-secondary-50 dark:bg-secondary-900/50 group-hover:bg-secondary-100 dark:group-hover:bg-secondary-800/50 transition-colors">
                <svg class="w-6 h-6 text-secondary-500 dark:text-secondary-400" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4" />
                </svg>
              </span>
            </div>
            <div class="grid grid-cols-2 gap-4">
              <div class="flex items-center p-3 bg-secondary-50 dark:bg-secondary-900/50 rounded-lg">
                <svg class="h-5 w-5 text-secondary-500 dark:text-secondary-400" fill="currentColor" viewBox="0 0 20 20">
                  <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                </svg>
                <span class="ml-2 text-gray-700 dark:text-gray-300">Frontend Development</span>
              </div>
              <div class="flex items-center p-3 bg-secondary-50 dark:bg-secondary-900/50 rounded-lg">
                <svg class="h-5 w-5 text-secondary-500 dark:text-secondary-400" fill="currentColor" viewBox="0 0 20 20">
                  <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                </svg>
                <span class="ml-2 text-gray-700 dark:text-gray-300">Backend Development</span>
              </div>
              <div class="flex items-center p-3 bg-secondary-50 dark:bg-secondary-900/50 rounded-lg">
                <svg class="h-5 w-5 text-secondary-500 dark:text-secondary-400" fill="currentColor" viewBox="0 0 20 20">
                  <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                </svg>
                <span class="ml-2 text-gray-700 dark:text-gray-300">Mobile Development</span>
              </div>
              <div class="flex items-center p-3 bg-secondary-50 dark:bg-secondary-900/50 rounded-lg">
                <svg class="h-5 w-5 text-secondary-500 dark:text-secondary-400" fill="currentColor" viewBox="0 0 20 20">
                  <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                </svg>
                <span class="ml-2 text-gray-700 dark:text-gray-300">Probleemoplossend Denken</span>
              </div>
            </div>
          </div>
        </div>

        <!-- Future Goals -->
        <div class="bg-white dark:bg-gray-800 rounded-2xl shadow-sm hover:shadow-xl transition-all duration-300 overflow-hidden border border-gray-100 dark:border-gray-700 group">
          <div class="p-6">
            <div class="flex items-center justify-between mb-4">
              <h2 class="text-xl font-semibold text-gray-900 dark:text-white group-hover:text-accent-500 dark:group-hover:text-accent-400 transition-colors">
                Toekomstdoelen
              </h2>
              <span class="flex items-center justify-center w-10 h-10 rounded-full bg-accent-50 dark:bg-accent-900/50 group-hover:bg-accent-100 dark:group-hover:bg-accent-800/50 transition-colors">
                <svg class="w-6 h-6 text-accent-500 dark:text-accent-400" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z" />
                </svg>
              </span>
            </div>
            <div class="space-y-4 text-gray-600 dark:text-gray-300">
              <p>
                Over 3 tot 5 jaar hoop ik als freelancer aan de slag te kunnen gaan, zodat ik op zelfstandige basis 
                projecten kan realiseren. Indien dit niet direct mogelijk is, wil ik graag starten bij een bekend 
                IT-bedrijf waar ik mij verder kan specialiseren als frontend of backend developer.
              </p>
              <p>
                Op lange termijn droom ik ervan om zelf een IT-bedrijf op te starten. Binnen een werkomgeving vind ik 
                respect, eerlijkheid en open communicatie erg belangrijk. Ik geloof dat een goede samenwerking en een 
                positieve sfeer bijdragen tot betere resultaten en persoonlijke groei.
              </p>
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