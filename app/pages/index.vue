<template>
  <div class="min-h-screen bg-gradient-to-br from-slate-900 via-purple-900 to-slate-900 relative overflow-hidden">
    <!-- Animated background elements -->
    <div class="absolute inset-0">
      <div class="absolute top-1/4 left-1/4 w-72 h-72 bg-emerald-500/20 rounded-full blur-3xl animate-pulse"/>
      <div class="absolute top-3/4 right-1/4 w-96 h-96 bg-purple-500/20 rounded-full blur-3xl animate-pulse delay-1000"/>
      <div
        class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 w-64 h-64 bg-blue-500/10 rounded-full blur-3xl animate-ping"/>
    </div>

    <!-- Floating particles -->
    <div class="absolute inset-0 overflow-hidden">
      <div class="absolute top-20 left-20 w-2 h-2 bg-emerald-400 rounded-full animate-bounce delay-300"/>
      <div class="absolute top-40 right-32 w-1 h-1 bg-purple-400 rounded-full animate-bounce delay-700"/>
      <div class="absolute bottom-32 left-1/3 w-1.5 h-1.5 bg-blue-400 rounded-full animate-bounce delay-1000"/>
      <div class="absolute top-1/3 right-20 w-1 h-1 bg-pink-400 rounded-full animate-bounce delay-500"/>
    </div>

    <!-- Main content -->
    <div class="relative z-10 flex flex-col items-center justify-center min-h-screen px-4">
      <!-- Hero section -->
      <div class="text-center space-y-8 max-w-4xl mx-auto">
        <!-- Logo/Brand with glow effect -->
        <div class="relative">
          <h1
            class="font-bold text-6xl md:text-8xl bg-gradient-to-r from-emerald-400 via-blue-500 to-purple-600 bg-clip-text text-transparent animate-pulse">
            wea.vin
          </h1>
          <div
            class="absolute inset-0 font-bold text-6xl md:text-8xl bg-gradient-to-r from-emerald-400 via-blue-500 to-purple-600 bg-clip-text text-transparent blur-2xl opacity-50 animate-pulse"/>
        </div>

        <!-- Subtitle with typewriter effect -->
        <div class="space-y-4">
          <p class="text-xl md:text-2xl text-slate-300 font-light leading-relaxed">
            Too bad, this page is not ready yet.
          </p>
        </div>

        <!-- Action buttons -->
        <div class="flex flex-col sm:flex-row items-center justify-center gap-4 pt-8">
          <UButton
label="Visit weavin.cn" icon="i-lucide-external-link" to="https://weavin.cn" target="_blank"
            size="lg" color="emerald" variant="solid"
            class="transform hover:scale-105 transition-all duration-300 shadow-lg hover:shadow-emerald-500/25" />
        </div>
      </div>

      <!-- Footer -->
      <div class="absolute bottom-8 left-1/2 transform -translate-x-1/2">
        <p class="text-slate-500 text-sm">© 2025 weavIntelli. Building the future.</p>
      </div>
    </div>
  </div>
</template>

<script setup>
// Add any reactive data or methods here if needed
useHead({
  title: 'wea.vin',
  meta: [
    { name: 'description', content: 'Revolutionary platform that weaves intelligence into every digital interaction. Coming soon.' }
  ]
})
</script>

<style scoped>
/* Custom animations */
@keyframes float {

  0%,
  100% {
    transform: translateY(0px);
  }

  50% {
    transform: translateY(-20px);
  }
}

.animate-float {
  animation: float 6s ease-in-out infinite;
}

/* Enhance the glow effect */
.text-glow {
  text-shadow: 0 0 20px rgba(16, 185, 129, 0.5);
}
</style>
