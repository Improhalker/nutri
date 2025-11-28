<template>
  <div class="w-full relative mx-auto max-w-[28rem] space-y-4">

    <!-- Gráfico / Chart -->
    <div class="relative aspect-video">
      <!-- Aqui você pode colocar seu gráfico, ou usar uma imagem placeholder -->
      <img
        src="https://media.inlead.cloud/uploads/40296/2025-10-24/lg-FqKJk-8020-quiz.png"
        alt="Gráfico do método 80/20"
        class="absolute inset-0 w-full h-full object-cover rounded-2xl"
      />
    </div>

    <!-- Card de estatística -->
    <div class="bg-green-100 text-green-700 p-4 rounded-2xl">
      <p>
        <em>87% de los usuarios</em> de la "Dieta 80/20" de Marta Gómez
        <strong>mantienen su pérdida de peso</strong> después de 6 meses
      </p>
    </div>

    <!-- Explicação / Texto -->
    <div class="text-gray-900">
      <p>
        💡 Esto es porque el plan te permite un 20% de comidas libres, 
        <strong>no es una dieta estricta más</strong>
      </p>
    </div>

    <!-- Botão de avançar -->
    <div class="mx-auto max-w-[28rem]">
      <button
        @click="$emit('next')"
        class="w-full rounded-2xl bg-green-600 text-white py-3 md:py-4 font-semibold shadow-sm hover:shadow-md active:scale-[.99] transition"
      >
        CONTINUAR  https://inlead.digital/metodo-8020/
      </button>
    </div>

  </div>
</template>
