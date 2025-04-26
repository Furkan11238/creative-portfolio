<template>
  <div class="min-h-screen bg-gradient-to-br from-white to-primary-50/30 dark:from-gray-900 dark:to-primary-900/30">
    <!-- Header -->
    <div class="relative py-24 overflow-hidden">
      <div class="absolute inset-0 bg-gradient-to-b from-primary-500/10 to-transparent dark:from-primary-500/5"></div>
      <div class="relative max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
        <h1 class="text-4xl md:text-5xl font-bold text-gray-900 dark:text-white text-center mb-4 animate-fade-in">
          Eindreflectie
        </h1>
        <p class="text-xl text-gray-600 dark:text-gray-300 text-center max-w-3xl mx-auto animate-slide-in">
          Een terugblik op mijn professionele reis en persoonlijke groei
        </p>
      </div>
    </div>

    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 pb-24">
      <div class="grid gap-8 md:grid-cols-2">
        <!-- Technische Ontwikkeling -->
        <div class="bg-white dark:bg-gray-800 rounded-2xl shadow-sm hover:shadow-xl transition-all duration-300 overflow-hidden border border-gray-100 dark:border-gray-700 group">
          <div class="p-6">
            <div class="flex items-center justify-between mb-4">
              <h2 class="text-xl font-bold text-gray-900 dark:text-white group-hover:text-primary-500 dark:group-hover:text-primary-400 transition-colors">
                Technische Ontwikkeling
              </h2>
              <span class="flex items-center justify-center w-10 h-10 rounded-full bg-primary-50 dark:bg-primary-900/50 group-hover:bg-primary-100 dark:group-hover:bg-primary-800/50 transition-colors">
                <svg class="w-6 h-6 text-primary-500 dark:text-primary-400" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4" />
                </svg>
              </span>
            </div>
            <p class="text-gray-600 dark:text-gray-300">
              De technische seminaries hebben mijn kennis aanzienlijk verbreed. Van moderne frameworks zoals Flutter tot enterprise architectuur en API testing, elk seminar bood nieuwe inzichten en praktische vaardigheden.
            </p>
            <p class="text-gray-600 dark:text-gray-300 mt-4">
              De Hack The Future challenge was een hoogtepunt, waar ik SAP-technologieën kon toepassen in een innovatief project. Deze ervaring heeft niet alleen mijn technische vaardigheden verbeterd, maar ook mijn vermogen om onder tijdsdruk te presteren.
            </p>
          </div>
        </div>

        <!-- Persoonlijke Groei -->
        <div class="bg-white dark:bg-gray-800 rounded-2xl shadow-sm hover:shadow-xl transition-all duration-300 overflow-hidden border border-gray-100 dark:border-gray-700 group">
          <div class="p-6">
            <div class="flex items-center justify-between mb-4">
              <h2 class="text-xl font-bold text-gray-900 dark:text-white group-hover:text-secondary-500 dark:group-hover:text-secondary-400 transition-colors">
                Persoonlijke Groei
              </h2>
              <span class="flex items-center justify-center w-10 h-10 rounded-full bg-secondary-50 dark:bg-secondary-900/50 group-hover:bg-secondary-100 dark:group-hover:bg-secondary-800/50 transition-colors">
                <svg class="w-6 h-6 text-secondary-500 dark:text-secondary-400" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z" />
                </svg>
              </span>
            </div>
            <p class="text-gray-600 dark:text-gray-300">
              De POP-sessies waren cruciaal voor mijn persoonlijke ontwikkeling. 'Brein aan het werk!' heeft me geleerd efficiënter om te gaan met digitale afleidingen, terwijl 'My Team and I' mijn begrip van teamdynamiek heeft verdiept.
            </p>
            <p class="text-gray-600 dark:text-gray-300 mt-4">
              De projectweek 2TIN was een intensieve periode van zelfreflectie en groei. Door de focus op academisch schrijven en teamwork heb ik niet alleen mijn communicatieve vaardigheden verbeterd, maar ook geleerd hoe ik effectiever kan samenwerken in diverse teams.
            </p>
          </div>
        </div>

        <!-- Internationale Dimensie -->
        <div class="bg-white dark:bg-gray-800 rounded-2xl shadow-sm hover:shadow-xl transition-all duration-300 overflow-hidden border border-gray-100 dark:border-gray-700 group">
          <div class="p-6">
            <div class="flex items-center justify-between mb-4">
              <h2 class="text-xl font-bold text-gray-900 dark:text-white group-hover:text-accent-500 dark:group-hover:text-accent-400 transition-colors">
                Internationale Dimensie
              </h2>
              <span class="flex items-center justify-center w-10 h-10 rounded-full bg-accent-50 dark:bg-accent-900/50 group-hover:bg-accent-100 dark:group-hover:bg-accent-800/50 transition-colors">
                <svg class="w-6 h-6 text-accent-500 dark:text-accent-400" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3.055 11H5a2 2 0 012 2v1a2 2 0 002 2 2 2 0 012 2v2.945M8 3.935V5.5A2.5 2.5 0 0010.5 8h.5a2 2 0 012 2 2 2 0 104 0 2 2 0 012-2h1.064M15 20.488V18a2 2 0 012-2h3.064M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
                </svg>
              </span>
            </div>
            <p class="text-gray-600 dark:text-gray-300">
              De IT-events in Amsterdam hebben mijn horizon verbreed en mijn netwerk internationaal uitgebreid. De VueJS en TC39 meetups boden niet alleen technische kennis, maar ook waardevolle contacten in de internationale tech-community.
            </p>
            <p class="text-gray-600 dark:text-gray-300 mt-4">
              Het culturele aspect, met het bezoek aan NEMO Science Museum, voegde een extra dimensie toe aan mijn begrip van technologie in een bredere maatschappelijke context.
            </p>
          </div>
        </div>

        <!-- Toekomstvisie -->
        <div class="bg-white dark:bg-gray-800 rounded-2xl shadow-sm hover:shadow-xl transition-all duration-300 overflow-hidden border border-gray-100 dark:border-gray-700 group">
          <div class="p-6">
            <div class="flex items-center justify-between mb-4">
              <h2 class="text-xl font-bold text-gray-900 dark:text-white group-hover:text-primary-500 dark:group-hover:text-primary-400 transition-colors">
                Blik op de Toekomst
              </h2>
              <span class="flex items-center justify-center w-10 h-10 rounded-full bg-primary-50 dark:bg-primary-900/50 group-hover:bg-primary-100 dark:group-hover:bg-primary-800/50 transition-colors">
                <svg class="w-6 h-6 text-primary-500 dark:text-primary-400" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M11.933 12.8a1 1 0 000-1.6L6.6 7.2A1 1 0 005 8v8a1 1 0 001.6.8l5.333-4zM19.933 12.8a1 1 0 000-1.6l-5.333-4A1 1 0 0013 8v8a1 1 0 001.6.8l5.333-4z" />
                </svg>
              </span>
            </div>
            <p class="text-gray-600 dark:text-gray-300">
              Deze ervaringen hebben mijn passie voor IT versterkt en mijn toekomstvisie verscherpt. Ik zie mezelf ontwikkelen in de richting van full-stack development met een focus op moderne technologieën en innovatie.
            </p>
            <p class="text-gray-600 dark:text-gray-300 mt-4">
              De combinatie van technische expertise en soft skills die ik heb opgedaan, vormt een sterke basis voor mijn verdere professionele groei.
            </p>
          </div>
        </div>
      </div>

      <!-- Conclusie -->
      <div class="mt-12 bg-gradient-to-br from-primary-50 to-secondary-50 dark:from-gray-800 dark:to-gray-700 rounded-2xl p-8">
        <h2 class="text-2xl font-bold text-gray-900 dark:text-white mb-4">Conclusie</h2>
        <p class="text-gray-600 dark:text-gray-300">
          Terugkijkend op dit jaar zie ik een duidelijke progressie in zowel mijn technische capaciteiten als persoonlijke ontwikkeling. De diverse activiteiten hebben elkaar perfect aangevuld en hebben bijgedragen aan een holistische groei als IT-professional. Ik kijk ernaar uit om deze kennis en ervaring toe te passen in toekomstige uitdagingen.
        </p>
      </div>
    </div>
  </div>
</template>

<script setup>
// No additional setup required for this page
</script>

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