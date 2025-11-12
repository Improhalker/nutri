<template>
  <div class="text-center">
    <h2 class="text-2xl font-semibold mb-6">Perfeito! Deixe seu e-mail abaixo 👇</h2>
    <input type="email" placeholder="Seu melhor e-mail" class="border p-2 rounded w-full mb-4" />
    <button class="bg-green-500 text-white px-6 py-2 rounded-xl">Enviar</button>
    <button @click="$emit('prev')" class="mt-4 text-gray-500 underline">Voltar</button>
  </div>
</template>
