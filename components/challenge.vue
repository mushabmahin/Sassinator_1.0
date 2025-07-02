<template>
  <div class="bg-gray-900 py-24 sm:py-32">
    <div class="mx-auto max-w-7xl px-6 lg:px-8">
      <div class="mx-auto max-w-2xl lg:text-center">
        <h2 class="text-base/7 font-semibold text-indigo-400">THE CHALLENGE</h2>
        <p class="mt-2 text-4xl font-semibold tracking-tight text-pretty text-white sm:text-5xl lg:text-balance">Are You Drowning in SaaS Bloat?</p>
        <p class="mt-6 text-lg/8 text-gray-300">Traditional SaaS solutions create more problems than they solve</p>
      </div>
      <div class="mx-auto mt-16 max-w-2xl sm:mt-20 lg:mt-24 lg:max-w-none">
        <dl class="grid max-w-xl grid-cols-1 gap-x-8 gap-y-16 lg:max-w-none lg:grid-cols-3">
          <div v-for="feature in features" :key="feature.name" class="flex flex-col">
            <dt class="flex items-center gap-x-3 text-base/7 font-semibold text-white">
              <component :is="feature.icon" class="size-5 flex-none text-indigo-400" aria-hidden="true" />
              {{ feature.name }}
            </dt>
            <dd class="mt-4 flex flex-auto flex-col text-base/7 text-gray-400">
              <p class="flex-auto">{{ feature.description }}</p>
            </dd>
          </div>
        </dl>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ArrowPathIcon, CloudArrowUpIcon, LockClosedIcon } from '@heroicons/vue/20/solid'

const features = [
  {
    name: 'Vendor Lock-In',
    description:
      'High recurring costs for limited utility with no easy exit strategy',
    icon: LockClosedIcon,
  },
  {
    name: 'Siloed Systems',
    description:
      "Tools that don't communicate, creating workflow bottlenecks",
    icon: ArrowPathIcon,
  },
  {
    name: 'Poor UX',
    description:
      'Low employee engagement with clunky, non-intuitive interfaces',
    icon: CloudArrowUpIcon,
  },
  {
    name: 'Slow Updates',
    description:
      'Feature rollout delays and backlog issues from vendors',
    icon: ArrowPathIcon,
  },
  {
    name: 'Adaptation Issues',
    description:
      'Inability to rapidly respond to new compliance or operational needs',
    icon: CloudArrowUpIcon,
  },
  {
    name: 'Hidden Costs',
    description:
      'Customization often costs 7-9x the SaaS license fee',
    icon: LockClosedIcon,
  },
]
</script>