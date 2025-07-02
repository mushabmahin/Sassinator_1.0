<template>
  <div class="bg-gray-900 py-24 sm:py-32">
    <div class="mx-auto max-w-7xl px-6 lg:px-8">
      <div class="mx-auto max-w-2xl lg:max-w-none">
        <div class="text-center">
          <h2 class="text-base/7 font-semibold text-indigo-400">WHY SAASINATOR?</h2>
          <p class="mt-2 text-4xl font-semibold tracking-tight text-balance text-white sm:text-5xl">Outcomes, Not Bloat</p>
          <p class="mt-4 text-lg/8 text-gray-300">The Saasinator difference for enterprise AI transformation</p>
        </div>
        <dl class="mt-16 grid grid-cols-1 gap-0.5 overflow-hidden rounded-2xl text-center sm:grid-cols-2 lg:grid-cols-3">
          <div v-for="stat in stats" :key="stat.id" class="flex flex-col bg-white/5 p-8">
            <dt class="text-lg font-semibold text-white">{{ stat.name }}</dt>
            <dd class="order-first text-2xl font-semibold tracking-tight text-indigo-400 mb-2">
              <component :is="stat.icon" class="mx-auto mb-2 size-12" aria-hidden="true" />
            </dd>
            <dd class="text-base text-gray-300">{{ stat.description }}</dd>
          </div>
        </dl>
      </div>
    </div>
  </div>
</template>

<script setup>
import { BanknotesIcon, ClockIcon, PuzzlePieceIcon, LockClosedIcon, AcademicCapIcon, BoltIcon } from '@heroicons/vue/20/solid'

const stats = [
  { id: 1, name: '30-50% Lower IT Spend', description: 'Replace expensive SaaS licenses with bespoke AI apps at a fraction of the cost', icon: BanknotesIcon },
  { id: 2, name: 'Accelerated ROI', description: 'Deploy custom AI agents in weeks, not months, delivering measurable impact fast', icon: ClockIcon },
  { id: 3, name: 'Tailored to Your Workflow', description: 'No generic features – only what drives your specific business value', icon: PuzzlePieceIcon },
  { id: 4, name: 'Own Your Innovation', description: 'No vendor lock-in, full control over your secure, compliant AI solutions', icon: LockClosedIcon },
  { id: 5, name: 'Strategic Advisor + Implementer', description: 'We audit your stack, identify high-ROI replacements, and deliver the AI alternative', icon: AcademicCapIcon },
  { id: 6, name: 'Agile Alternative to Big SIs', description: 'Faster, more experimental, and outcome-driven than traditional system integrators', icon: BoltIcon },
]
</script>