<template>
    <div class="bg-gray-900 py-24 sm:py-32">
      <div class="mx-auto max-w-7xl px-6 lg:px-8">
        <div class="mx-auto max-w-2xl lg:mx-0">
          <h2 class="text-4xl font-semibold tracking-tight text-pretty text-white sm:text-5xl">AI Agents in Action</h2>
          <p class="mt-6 text-lg/8 text-gray-300">Transformative results across industries</p>
        </div>
        <div class="mx-auto mt-16 max-w-2xl sm:mt-20 lg:mt-24 lg:max-w-none">
          <dl class="grid max-w-xl grid-cols-1 gap-x-8 gap-y-16 lg:max-w-none lg:grid-cols-3">
            <div v-for="feature in features" :key="feature.name" class="flex flex-col">
              <dt class="text-base/7 font-semibold text-white">
                <div class="mb-6 flex size-10 items-center justify-center rounded-lg bg-indigo-500">
                  <component :is="feature.icon" class="size-6 text-white" aria-hidden="true" />
                </div>
                {{ feature.name }}
                <div class="text-xs font-normal text-gray-300">{{ feature.subtitle }}</div>
              </dt>
              <dd class="mt-1 flex flex-auto flex-col text-base/7 text-gray-400">
                <p class="flex-auto" v-html="feature.description"></p>
              </dd>
            </div>
          </dl>
        </div>
      </div>
    </div>
  </template>
  
  <script setup>
  import { ShoppingCartIcon, ComputerDesktopIcon, DocumentTextIcon, TruckIcon, ClipboardDocumentCheckIcon, UserGroupIcon } from '@heroicons/vue/24/outline'
  
  const features = [
    {
      name: 'AI Expense Auditor',
      subtitle: 'Retail Client',
      description:
        'Replaced SAP Concur, cutting reimbursement cycle time by <b>80%</b> and saving <b>$1.2M annually</b> in labor costs.',
      icon: ShoppingCartIcon,
    },
    {
      name: 'Intelligent IT Support Agent',
      subtitle: 'Healthcare Provider',
      description:
        'Automated <b>70% of Tier-1 support queries</b>, reducing average resolution time by <b>65%</b> and improving user satisfaction.',
      icon: ComputerDesktopIcon,
    },
    {
      name: 'AI Sales Proposal Generator',
      subtitle: 'BFSI Client',
      description:
        'Enabled sales teams to generate custom proposals <b>5X faster</b>, leading to a <b>22% increase</b> in conversion rates.',
      icon: DocumentTextIcon,
    },
    {
      name: 'AI Supply Chain Assistant',
      subtitle: 'Manufacturing/Logistics',
      description:
        'Replaced clunky ERP add-ons, optimizing inventory forecasting and logistics routing, leading to <b>18% efficiency gains</b>.',
      icon: TruckIcon,
    },
    {
      name: 'AI Document Compliance Checker',
      subtitle: 'Public Sector',
      description:
        'Automated review of complex regulations, ensuring <b>99% compliance</b> and reducing manual audit time by <b>75%</b>.',
      icon: ClipboardDocumentCheckIcon,
    },
    {
      name: 'AI HR Onboarding Assistant',
      subtitle: 'Technology Company',
      description:
        'Reduced new hire onboarding time from <b>2 weeks to 3 days</b> while improving satisfaction scores by <b>40%</b>.',
      icon: UserGroupIcon,
    },
  ]
  </script>