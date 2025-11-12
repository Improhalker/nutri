<template>
  <div class="text-center">
    <h2 class="text-2xl font-semibold mb-6">Qual é o seu nível atual?</h2>
    <div class="flex flex-col gap-3">
      <button @click="$emit('next')" class="bg-blue-500 text-white px-6 py-2 rounded-xl">Iniciante</button>
      <button @click="$emit('next')" class="bg-blue-500 text-white px-6 py-2 rounded-xl">Intermediário</button>
      <button @click="$emit('next')" class="bg-blue-500 text-white px-6 py-2 rounded-xl">Avançado</button>
    </div>
    <button @click="$emit('prev')" class="mt-4 text-gray-500 underline">Voltar</button>
  </div>
</template>
