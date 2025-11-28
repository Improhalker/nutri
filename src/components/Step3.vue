<template>
  <div class="flex flex-row flex-wrap -mx-1">
    
    <!-- Texto 1 -->
    <div class="w-full px-1">
      <h2 class="text-center text-lg md:text-xl font-semibold leading-tight">
        Nuestro método
        <span class="text-green-600"> RESUELVE ESO </span>
        <span class="text-gray-900">para tí</span>
      </h2>
    </div>

    <!-- Texto 2 -->
    <div class="w-full px-1 mt-2">
      <h1 class="text-center text-red-600 text-xl md:text-2xl font-extrabold">
        COMO FUNCIONA EL MÉTODO 80/20
      </h1>
    </div>

    <!-- Imagem -->
    <div class="w-full px-1 mt-4">
      <div class="relative w-full rounded-2xl overflow-hidden pb-[70.9615%]">
        <img src="https://media.inlead.cloud/uploads/40296/2025-10-24/lg-FqKJk-8020-quiz.png"
          alt="Ilustração do método 80/20" class="absolute inset-0 w-full h-full object-cover" />
      </div>
    </div>

    <!-- Botão -->
    <div class="w-full px-1 mt-4">
      <div class="mx-auto max-w-[28rem]">
        <button
          type="button"
          @click="$emit('next')"
          class="w-full rounded-2xl bg-green-600 text-white py-3 md:py-4 font-semibold shadow-sm hover:shadow-md active:scale-[.99] transition"
        >
          CONTINUAR
        </button>

      </div>
    </div>

  </div>

</template>
