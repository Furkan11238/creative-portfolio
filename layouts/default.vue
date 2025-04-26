<template>
  <div class="min-h-screen bg-gray-50 dark:bg-gray-900">
    <!-- Navigation -->
    <nav class="fixed top-0 w-full bg-white/80 dark:bg-gray-800/80 backdrop-blur-sm z-50 shadow-sm">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="flex justify-between h-16">
          <div class="flex">
            <div class="flex-shrink-0 flex items-center">
              <h1 class="text-xl font-bold text-gray-900 dark:text-white">Mehmet Furkan</h1>
            </div>
          </div>
          <div class="flex items-center">
            <div class="hidden md:ml-6 md:flex md:space-x-8">
              <NuxtLink to="/" class="nav-link">Home</NuxtLink>
              <NuxtLink to="/about" class="nav-link">Over Mij</NuxtLink>
              <NuxtLink to="/activities" class="nav-link">Activiteiten</NuxtLink>
              <NuxtLink to="/projects" class="nav-link">Projecten</NuxtLink>
              <button @click="toggleTheme" class="p-2 rounded-lg hover:bg-gray-100 dark:hover:bg-gray-700">
                <span class="dark:hidden">🌙</span>
                <span class="hidden dark:inline">☀️</span>
              </button>
            </div>
          </div>
        </div>
      </div>
    </nav>

    <!-- Main Content -->
    <main class="pt-16">
      <slot />
    </main>

    <!-- Footer -->
    <footer class="bg-white dark:bg-gray-800 mt-12">
      <div class="max-w-7xl mx-auto py-12 px-4 sm:px-6 lg:px-8">
        <div class="text-center">
          <p class="text-gray-500 dark:text-gray-400">© 2024 Mehmet Furkan Karakoc. Alle rechten voorbehouden.</p>
        </div>
      </div>
    </footer>
  </div>
</template>

<script setup lang="ts">
const colorMode = useColorMode()

const toggleTheme = () => {
  colorMode.preference = colorMode.value === 'dark' ? 'light' : 'dark'
}
</script>

<style>
.nav-link {
  @apply inline-flex items-center px-1 pt-1 text-sm font-medium text-gray-500 dark:text-gray-300 hover:text-gray-900 dark:hover:text-white border-b-2 border-transparent hover:border-gray-300 dark:hover:border-gray-600;
}

.nav-link.router-link-active {
  @apply border-blue-500 text-gray-900 dark:text-white;
}
</style> 