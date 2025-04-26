<template>
  <div class="min-h-screen bg-gray-50 dark:bg-gray-900 py-12">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 space-y-12">
      <!-- Filter Controls -->
      <div class="flex flex-wrap gap-4 mb-8">
        <button
          v-for="filter in filters"
          :key="filter.id"
          @click="activeFilter = filter.id"
          :class="[
            'px-4 py-2 rounded-full text-sm font-medium transition-all duration-300',
            activeFilter === filter.id
              ? 'bg-primary-500 text-white dark:bg-primary-400 dark:text-gray-900'
              : 'bg-white dark:bg-gray-800 text-gray-700 dark:text-gray-300 hover:bg-primary-50 dark:hover:bg-primary-900/50'
          ]"
        >
          {{ filter.name }}
        </button>
      </div>

      <!-- Seminars -->
      <section v-show="activeFilter === 'all' || activeFilter === 'seminars'" class="transform transition-all duration-500">
        <div class="flex items-center space-x-4 mb-8">
          <h2 class="text-2xl font-bold text-gray-900 dark:text-white">Seminars</h2>
          <div class="h-px flex-1 bg-gradient-to-r from-primary-500/50 to-transparent dark:from-primary-400/50"></div>
        </div>
        <div class="grid gap-6 md:grid-cols-2 lg:grid-cols-3">
          <div
            v-for="seminar in seminars"
            :key="seminar.title"
            class="bg-white dark:bg-gray-800 rounded-2xl shadow-sm hover:shadow-xl transition-all duration-300 overflow-hidden border border-gray-100 dark:border-gray-700 hover:border-primary-500 dark:hover:border-primary-400 group"
          >
            <div class="p-6">
              <div class="flex items-center justify-between mb-4">
                <h3 class="text-lg font-semibold text-gray-900 dark:text-white group-hover:text-primary-500 dark:group-hover:text-primary-400 transition-colors">
                  {{ seminar.title }}
                </h3>
              </div>
              <p class="text-gray-600 dark:text-gray-300 text-sm">
                {{ seminar.description }}
              </p>
              <div class="mt-4 pt-4 border-t border-gray-100 dark:border-gray-700">
                <div class="flex items-center justify-between text-sm">
                  <div class="flex items-center text-gray-500 dark:text-gray-400">
                    <CalendarIcon class="w-4 h-4 mr-2" />
                    {{ seminar.date }}
                  </div>
                  <div class="flex items-center text-gray-500 dark:text-gray-400">
                    <MapPinIcon class="w-4 h-4 mr-2" />
                    {{ seminar.location }}
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>

      <!-- Innovation -->
      <section v-show="activeFilter === 'all' || activeFilter === 'innovation'" class="transform transition-all duration-500">
        <div class="flex items-center space-x-4 mb-8">
          <h2 class="text-2xl font-bold text-gray-900 dark:text-white">Innovatie</h2>
          <div class="h-px flex-1 bg-gradient-to-r from-accent-500/50 to-transparent dark:from-accent-400/50"></div>
        </div>
        <div class="grid gap-6 lg:grid-cols-2">
          <div class="bg-white dark:bg-gray-800 rounded-2xl shadow-sm hover:shadow-xl transition-all duration-300 overflow-hidden border border-gray-100 dark:border-gray-700 group">
            <div class="p-6">
              <div class="flex items-center justify-between mb-4">
                <h3 class="text-lg font-semibold text-gray-900 dark:text-white group-hover:text-accent-500 dark:group-hover:text-accent-400 transition-colors">
                  Application Integration
                </h3>
                <span class="flex items-center justify-center w-10 h-10 rounded-full bg-accent-50 dark:bg-accent-900/50 group-hover:bg-accent-100 dark:group-hover:bg-accent-800/50 transition-colors">
                  <CodeBracketIcon class="w-5 h-5 text-accent-500 dark:text-accent-400" />
                </span>
              </div>
              <p class="text-gray-600 dark:text-gray-300 text-sm">
                Kennismaking met verschillende integratie-technologieën en -platformen zoals Red Hat Camel en Azure API Management. Focus op API ontwikkeling en beheer binnen complexe softwareomgevingen.
              </p>
              <div class="mt-4 pt-4 border-t border-gray-100 dark:border-gray-700">
                <div class="flex items-center justify-between text-sm">
                  <div class="flex items-center text-gray-500 dark:text-gray-400">
                    <CalendarIcon class="w-4 h-4 mr-2" />
                    24 september - 8 oktober 2024
                  </div>
                  <div class="flex items-center text-gray-500 dark:text-gray-400">
                    <MapPinIcon class="w-4 h-4 mr-2" />
                    Corda Campus
                  </div>
                </div>
              </div>
            </div>
          </div>

          <div class="bg-white dark:bg-gray-800 rounded-2xl shadow-sm hover:shadow-xl transition-all duration-300 overflow-hidden border border-gray-100 dark:border-gray-700 group">
            <div class="p-6">
              <div class="flex items-center justify-between mb-4">
                <h3 class="text-lg font-semibold text-gray-900 dark:text-white group-hover:text-accent-500 dark:group-hover:text-accent-400 transition-colors">
                  Hack The Future 2024
                </h3>
                <span class="flex items-center justify-center w-10 h-10 rounded-full bg-accent-50 dark:bg-accent-900/50 group-hover:bg-accent-100 dark:group-hover:bg-accent-800/50 transition-colors">
                  <RocketLaunchIcon class="w-5 h-5 text-accent-500 dark:text-accent-400" />
                </span>
              </div>
              <p class="text-gray-600 dark:text-gray-300 text-sm">
                Ontwikkeling van een webapplicatie met SAP-technologieën voor het organiseren van expedities naar verre sterrenstelsels tijdens de Flexso Challenge.
              </p>
              <div class="mt-4 pt-4 border-t border-gray-100 dark:border-gray-700">
                <div class="flex items-center justify-between text-sm">
                  <div class="flex items-center text-gray-500 dark:text-gray-400">
                    <CalendarIcon class="w-4 h-4 mr-2" />
                    19 november 2024
                  </div>
                  <div class="flex items-center text-gray-500 dark:text-gray-400">
                    <MapPinIcon class="w-4 h-4 mr-2" />
                    Antwerpen
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>

      <!-- Personal Development -->
      <section v-show="activeFilter === 'all' || activeFilter === 'personal'" class="transform transition-all duration-500">
        <div class="flex items-center space-x-4 mb-8">
          <h2 class="text-2xl font-bold text-gray-900 dark:text-white">Persoonlijke Ontwikkeling</h2>
          <div class="h-px flex-1 bg-gradient-to-r from-secondary-500/50 to-transparent dark:from-secondary-400/50"></div>
        </div>
        <div class="grid gap-6 lg:grid-cols-2">
          <div class="bg-white dark:bg-gray-800 rounded-2xl shadow-sm hover:shadow-xl transition-all duration-300 overflow-hidden border border-gray-100 dark:border-gray-700 group">
            <div class="p-6">
              <div class="flex items-center justify-between mb-4">
                <h3 class="text-lg font-semibold text-gray-900 dark:text-white group-hover:text-secondary-500 dark:group-hover:text-secondary-400 transition-colors">
                  Projectweek 2TIN
                </h3>
                <span class="flex items-center justify-center w-10 h-10 rounded-full bg-secondary-50 dark:bg-secondary-900/50 group-hover:bg-secondary-100 dark:group-hover:bg-secondary-800/50 transition-colors">
                  <UserGroupIcon class="w-5 h-5 text-secondary-500 dark:text-secondary-400" />
                </span>
              </div>
              <p class="text-gray-600 dark:text-gray-300 text-sm">
                Interactieve sessies en workshops gericht op persoonlijke en professionele ontwikkeling, waaronder teamwork, reflectie en academisch schrijven.
              </p>
              <div class="mt-4 pt-4 border-t border-gray-100 dark:border-gray-700">
                <div class="flex items-center text-sm text-gray-500 dark:text-gray-400">
                  <CalendarIcon class="w-4 h-4 mr-2" />
                  12-16 februari 2024
                </div>
              </div>
            </div>
          </div>

          <div class="bg-white dark:bg-gray-800 rounded-2xl shadow-sm hover:shadow-xl transition-all duration-300 overflow-hidden border border-gray-100 dark:border-gray-700">
            <div class="p-6">
              <div class="flex items-center justify-between mb-4">
                <h3 class="text-lg font-semibold text-gray-900 dark:text-white">POP-sessies</h3>
                <span class="flex items-center justify-center w-10 h-10 rounded-full bg-secondary-50 dark:bg-secondary-900/50">
                  <LightBulbIcon class="w-5 h-5 text-secondary-500 dark:text-secondary-400" />
                </span>
              </div>
              <div class="space-y-4">
                <div class="group/item">
                  <h4 class="font-medium text-gray-900 dark:text-white group-hover/item:text-secondary-500 dark:group-hover/item:text-secondary-400 transition-colors">
                    Brein aan het werk! Niet storen!
                  </h4>
                  <p class="mt-1 text-sm text-gray-600 dark:text-gray-300">
                    Effect van digitale connectiviteit op onze hersenen en strategieën voor efficiënter werken.
                  </p>
                  <div class="mt-2 text-sm text-gray-500 dark:text-gray-400">5 maart 2024</div>
                </div>
                <div class="group/item">
                  <h4 class="font-medium text-gray-900 dark:text-white group-hover/item:text-secondary-500 dark:group-hover/item:text-secondary-400 transition-colors">
                    POPping
                  </h4>
                  <p class="mt-1 text-sm text-gray-600 dark:text-gray-300">
                    Zelfinzicht, feedback en het opstellen van een persoonlijk ontwikkelingsplan.
                  </p>
                  <div class="mt-2 text-sm text-gray-500 dark:text-gray-400">7 maart 2024</div>
                </div>
                <div class="group/item">
                  <h4 class="font-medium text-gray-900 dark:text-white group-hover/item:text-secondary-500 dark:group-hover/item:text-secondary-400 transition-colors">
                    My Team and I
                  </h4>
                  <p class="mt-1 text-sm text-gray-600 dark:text-gray-300">
                    Verdieping in teamwerking via de modellen van Lencioni en Tuckman.
                  </p>
                  <div class="mt-2 text-sm text-gray-500 dark:text-gray-400">9 oktober 2024</div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>

      <!-- Internationalization -->
      <section v-show="activeFilter === 'all' || activeFilter === 'international'" class="transform transition-all duration-500">
        <div class="flex items-center space-x-4 mb-8">
          <h2 class="text-2xl font-bold text-gray-900 dark:text-white">Internationalisering</h2>
          <div class="h-px flex-1 bg-gradient-to-r from-primary-500/50 to-transparent dark:from-primary-400/50"></div>
        </div>
        <div class="bg-white dark:bg-gray-800 rounded-2xl shadow-sm hover:shadow-xl transition-all duration-300 overflow-hidden border border-gray-100 dark:border-gray-700">
          <div class="p-6">
            <div class="flex items-center justify-between mb-6">
              <h3 class="text-lg font-semibold text-gray-900 dark:text-white">IT-events Amsterdam</h3>
              <span class="flex items-center justify-center w-10 h-10 rounded-full bg-primary-50 dark:bg-primary-900/50">
                <GlobeEuropeAfricaIcon class="w-5 h-5 text-primary-500 dark:text-primary-400" />
              </span>
            </div>
            <p class="text-gray-600 dark:text-gray-300 text-sm mb-6">
              Deelname aan twee vooraanstaande IT-events in Amsterdam, gericht op moderne webtechnologieën, gecombineerd met een cultureel bezoek.
            </p>
            <div class="grid gap-4 md:grid-cols-3">
              <div class="bg-gray-50 dark:bg-gray-700/50 rounded-xl p-4">
                <h4 class="font-medium text-gray-900 dark:text-white mb-2">VueJS Amsterdam Meetup</h4>
                <p class="text-sm text-gray-600 dark:text-gray-300">Netwerken en kennisdeling bij Funda HQ</p>
              </div>
              <div class="bg-gray-50 dark:bg-gray-700/50 rounded-xl p-4">
                <h4 class="font-medium text-gray-900 dark:text-white mb-2">TC39 JavaScript Meetup</h4>
                <p class="text-sm text-gray-600 dark:text-gray-300">Toekomst van JavaScript bij JetBrains</p>
              </div>
              <div class="bg-gray-50 dark:bg-gray-700/50 rounded-xl p-4">
                <h4 class="font-medium text-gray-900 dark:text-white mb-2">NEMO Science Museum</h4>
                <p class="text-sm text-gray-600 dark:text-gray-300">Interactieve technologie-expositie</p>
              </div>
            </div>
            <div class="mt-6 flex items-center justify-between text-sm">
              <div class="flex items-center text-gray-500 dark:text-gray-400">
                <CalendarIcon class="w-4 h-4 mr-2" />
                11-12 maart 2025
              </div>
              <div class="flex items-center text-gray-500 dark:text-gray-400">
                <MapPinIcon class="w-4 h-4 mr-2" />
                Amsterdam, Nederland
              </div>
            </div>
          </div>
        </div>
      </section>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import { CalendarIcon, MapPinIcon, CodeBracketIcon, RocketLaunchIcon, UserGroupIcon, LightBulbIcon, GlobeEuropeAfricaIcon } from '@heroicons/vue/24/outline'

const activeFilter = ref('all')

const filters = [
  { id: 'all', name: 'Alle Activiteiten' },
  { id: 'seminars', name: 'Seminaries' },
  { id: 'innovation', name: 'Innovatie' },
  { id: 'personal', name: 'Persoonlijke Ontwikkeling' },
  { id: 'international', name: 'Internationalisering' }
]

const seminars = [
  {
    title: 'The role of Power Apps',
    description: 'Ontwikkeling van moderne applicaties binnen Microsoft 365 met Power Apps.',
    date: '12 maart 2023',
    location: 'PXL, G412',
    icon: 'LightningBoltIcon'
  },
  {
    title: 'API & Security Testing',
    description: 'Technieken voor API testing en security testing, met focus op manuele tests.',
    date: '19 maart 2024',
    location: 'PXL, G412',
    icon: 'ShieldCheckIcon'
  },
  {
    title: 'ChatGPT implementaties',
    description: 'Inzetten van ChatGPT binnen bedrijven met praktijkvoorbeelden.',
    date: '23 april 2024',
    location: 'PXL, G414',
    icon: 'ChatBubbleBottomCenterIcon'
  },
  {
    title: 'The Rise of Low Code',
    description: 'Bouwen van een mobiele applicatie via het OutSystems platform.',
    date: '7 mei 2024',
    location: 'PXL, G412',
    icon: 'CubeIcon'
  },
  {
    title: 'Flutter en Use Case',
    description: 'Introductie tot Flutter voor cross-platform app development.',
    date: '6 november 2024',
    location: 'Corda Campus',
    icon: 'DevicePhoneMobileIcon'
  },
  {
    title: 'Enterprise Architecture',
    description: 'Creëren van stabiliteit in een veranderende technologische omgeving.',
    date: '20 november 2024',
    location: 'Corda Campus',
    icon: 'CircleStackIcon'
  },
  {
    title: 'Workshop Facilitation',
    description: 'Design Sprint methodologie en efficiënt faciliteren van workshops.',
    date: '4 december 2024',
    location: 'Corda Campus',
    icon: 'UserGroupIcon'
  },
  {
    title: 'State Management Angular',
    description: 'Nieuwe technieken zoals signals voor efficiënter state management.',
    date: '11 december 2024',
    location: 'Corda Campus',
    icon: 'ArrowPathIcon'
  }
]
</script>

<style scoped>
.transform {
  opacity: 0;
  animation: fadeIn 0.5s ease-out forwards;
}

@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

section {
  scroll-margin-top: 2rem;
}
</style>