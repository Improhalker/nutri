<template>
  <div class="text-center">
    <h2 class="text-2xl font-semibold mb-6">Você gostaria de aprender a desenhar animes?</h2>
    <div class="flex gap-4 justify-center">
      <button @click="$emit('next')" class="text-gray-800 px-6 py-2 rounded-xl">Sim</button>
      <button @click="$emit('next')" class=" text-gray-800 px-6 py-2 rounded-xl">Não</button>
    </div>
  </div>
</template>
