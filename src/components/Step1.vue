<template>
  <div class="text-center">
    <div class="w-full mx-auto max-w-[28rem] relative p-4">
      
      <!-- Título -->
      <div class="text-gray-900 py-4">
        <h1 class="text-center text-2xl font-bold leading-tight">
          ¿Cómo describirías tu
          <span class="text-green-500">cuerpo HOY</span>?
        </h1>

        <p class="text-center mt-1 text-sm opacity-90">
          Elegí la opción que más se adapta a vos
        </p>
      </div>

      <!-- Lista -->
      <div class="grid gap-3 mt-4">

        <!-- Regular -->
        <button
          @click="$emit('next', 'Regular')"
          class="flex items-center gap-3 bg-white/90 rounded-2xl overflow-hidden shadow-md active:scale-[.98] transition">
          <div class="min-w-[4rem] max-w-[5rem] bg-gray-50">
            <img src="https://media.inlead.cloud/uploads/40296/2025-10-23/xs-FSuha-screenshot-2025-10-23-at-40923-pm.png"
              class="w-full h-full object-cover">
          </div>
          <div class="flex-1 p-3">
            <p class="text-gray-800 font-semibold">Regular</p>
          </div>
        </button>

        <!-- Flácido -->
        <button
          @click="$emit('next', 'Flácido')"
          class="flex items-center gap-3 bg-white/90 rounded-2xl overflow-hidden shadow-md active:scale-[.98] transition">
          <div class="min-w-[4rem] max-w-[5rem] bg-gray-50">
            <img src="https://media.inlead.cloud/uploads/40296/2025-10-23/xs-FxAOO-screenshot-2025-10-23-at-40930-pm.png"
              class="w-full h-full object-cover">
          </div>
          <div class="flex-1 p-3">
            <p class="text-gray-800 font-semibold">Flácido</p>
          </div>
        </button>

        <!-- Sobrepeso -->
        <button
          @click="$emit('next', 'Sobrepeso')"
          class="flex items-center gap-3 bg-white/90 rounded-2xl overflow-hidden shadow-md active:scale-[.98] transition">
          <div class="min-w-[4rem] max-w-[5rem] bg-gray-50">
            <img src="https://media.inlead.cloud/uploads/40296/2025-10-23/xs-Owqeo-screenshot-2025-10-23-at-40937-pm.png"
              class="w-full h-full object-cover">
          </div>
          <div class="flex-1 p-3">
            <p class="text-gray-800 font-semibold">Sobrepeso</p>
          </div>
        </button>

      </div>
    </div>
  </div>
</template>
