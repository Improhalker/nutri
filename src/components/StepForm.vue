<template>
  <component :is="steps[currentStep]" @next="next" @prev="prev" />
</template>

<script setup>
import { ref } from 'vue'
import Step1 from './Step1.vue'
import Step2 from './Step2.vue'
import Step3 from './Step3.vue'
import Step4 from './Step4.vue'

const steps = [Step1, Step2, Step3, Step4]
const currentStep = ref(0)

const next = () => {
  if (currentStep.value < steps.length - 1) currentStep.value++
}
const prev = () => {
  if (currentStep.value > 0) currentStep.value--
}
</script>
