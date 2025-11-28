<template>
  <div class="text-center">
    <div class="w-full mx-auto max-w-[28rem] relative p-4">

      <!-- TÍTULO -->
      <div class="text-gray-900 py-4">
        <h1 class="text-center text-2xl font-bold leading-tight">
          ¿Qué te <span class="text-red-600">impide</span>
          <span class="text-green-600"> bajar de peso</span>?
        </h1>

        <p class="text-center mt-1 text-sm opacity-90">
          Podés elegir más de una opción
        </p>
      </div>

      <!-- LISTA -->
      <div class="grid grid-cols-1 gap-2 mt-2">

        <!-- ITEM -->
        <button
          v-for="(item, i) in options"
          :key="i"
          @click="toggle(item.value)"
          class="flex items-center text-left rounded-2xl overflow-hidden shadow-md border transition-all cursor-pointer"

          :class="selected.includes(item.value)
            ? 'bg-green-100 border-green-500 scale-[1.03]'
            : 'bg-white/90 border-gray-200 active:scale-[.97]'"
        >
          <!-- Emoji -->
          <div class="w-[3.75rem] flex justify-center items-center">
            <div class="text-3xl p-2">
              {{ item.icon }}
            </div>
          </div>

          <!-- Texto -->
          <div class="flex-1 p-3 pl-0 flex justify-between items-center gap-3">
            <p
              class="text-[1rem] leading-tight transition"
              :class="selected.includes(item.value) ? 'text-green-800 font-semibold' : 'text-gray-800'"
            >
              {{ item.label }}
            </p>

            <!-- Letra -->
            <div class="py-1">
              <div
                class="rounded-md min-w-[1.55rem] min-h-[1.55rem] px-2 py-[0.25rem] text-center text-xs font-medium transition"
                :class="selected.includes(item.value)
                  ? 'bg-green-600 text-white'
                  : 'bg-gray-200 text-gray-700'"
              >
                {{ letters[i] }}
              </div>
            </div>
          </div>
        </button>

      </div>

      <!-- BOTÃO CONTINUAR -->
      <div class="mt-4 mx-auto max-w-[28rem]">
        <button
          @click="confirm"
          :disabled="selected.length === 0"
          class="w-full py-3 rounded-2xl font-semibold transition-all"

          :class="selected.length
            ? 'bg-green-600 text-white active:scale-[.98]'
            : 'bg-gray-300 text-gray-500 cursor-not-allowed'"
        >
          CONTINUAR
        </button>
      </div>

    </div>
  </div>
</template>

<script setup>
import { ref } from "vue"

const letters = ["A", "B", "C", "D", "E", "F"]

const options = [
  { icon: "😣", label: "No logro controlar la ansiedad ni los atracones", value: "ansiedad" },
  { icon: "🍔", label: "Tengo hambre todo el tiempo", value: "hambre" },
  { icon: "💦", label: "Retención de líquidos/me siento hinchada", value: "retencion" },
  { icon: "🕒", label: "No tengo tiempo para cocinar", value: "tiempo" },
  { icon: "🤷‍♀️", label: "No sé qué comer", value: "que_comer" },
  { icon: "❓", label: "No sé cocinar", value: "cocinar" }
]

const selected = ref([])

const toggle = (val) => {
  if (selected.value.includes(val)) {
    selected.value = selected.value.filter((v) => v !== val)
  } else {
    selected.value.push(val)
  }
}

const emit = defineEmits(["next"])

const confirm = () => {
  emit("next", selected.value)
}
</script>
